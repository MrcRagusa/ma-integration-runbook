# Email and Collaboration Handover

## The day-one position

Email continues to flow to acquired-company addresses. Calendar invites continue to work. Existing chat platforms continue to operate. Any cross-company collaboration in the first 24 to 48 hours uses temporary mechanisms, typically guest access or external email, rather than rushed integrations.

The temptation on day one is to make email and collaboration tools the visible symbol of integration. New email signatures, new domain branding, new chat channels. Resist this. The acquired company's users need to do their actual jobs on day one, and changing the tools they use to communicate is the fastest way to make that harder.

## Sequencing decisions

Three decisions shape how email and collaboration migration plays out, and they're usually best made during pre-close rather than post-close.

**Domain strategy.** Will acquired users keep their existing email domain, move to the parent's domain, or end up with both during a transition? In most full-absorption integrations, the eventual answer is that acquired users get parent-company addresses. The question is whether that happens early (assertive integration) or late (more gradual). Early creates more visible change but resolves the question; late preserves continuity but extends the integration tail.

**Tenant strategy.** For Microsoft 365 acquirers, the question is whether to migrate the acquired tenant fully into the parent tenant, leave the acquired tenant operating indefinitely, or maintain a multi-tenant architecture deliberately. Full migration is the default for full-absorption integrations. Multi-tenant is sometimes appropriate for deals where acquired entities have specific data residency or regulatory requirements.

**Collaboration platform consolidation.** If the parent uses Teams and the acquired company uses Slack, or vice versa, a decision needs to be made early about which platform survives. Running both indefinitely creates visible friction and divides the workforce. Consolidating creates user-facing change and resistance, particularly if the platform being retired was loved by its users. Neither answer is wrong; the wrong move is leaving the question unanswered for months.

## Mailbox migration

Mailbox migration is the single most user-affecting technical task in most integrations. It's worth treating it as a project in its own right within wave 1 or wave 2.

The mechanical work involves moving mailbox content, including emails, folders, rules, signatures, and contacts, from the source tenant to the destination tenant. There are multiple tools available, including native Microsoft tooling, third-party tools like BitTitan, Quadrotech, or SkyKick, and custom scripted approaches. The right tool depends on the size of the migration and the budget.

The non-mechanical work is what makes or breaks the migration:

**Communication.** Users need to know when their migration is happening, what they need to do beforehand, what to expect during, and what changes after. Generic communications don't work; users need specifics.

**Pilot waves.** The first migration wave should be the IT team and a small group of senior leadership volunteers. Lessons from the pilot inform the broader rollout. Migrating regular users in the first wave creates avoidable visibility on whatever goes wrong.

**Mobile device reconfiguration.** Mailbox migration usually requires users to reconfigure their phones to point at the new mailbox. This is one of the most common sources of post-migration support tickets. Provide clear instructions, ideally with screenshots.

**Calendar handling.** Calendar invitations sent before migration but for events after migration sometimes don't track correctly. Test this before broad rollout and have a plan for the edge cases.

**Shared mailboxes and distribution lists.** These often get forgotten in initial migration scoping and surface as urgent issues during cutover. Inventory them deliberately.

**Public folders.** Older Exchange environments may still have public folders in active use. These migrate poorly and may need to be replaced with SharePoint or Teams alternatives during integration.

## Teams and chat platform consolidation

Where both companies use Microsoft Teams, the consolidation work is mostly about merging the underlying tenants and migrating Teams content alongside mailboxes. Teams membership, channels, files, and chat history all need to move. Chat history migration in particular has historically been imperfect; communicate this to users so they can save anything critical before migration.

Where one company uses Teams and the other uses Slack, or where chat platforms differ in other ways, the consolidation is messier. The two patterns I've seen work:

**Phased adoption.** The retiring platform is left operational but stops being used for official communications. Users are given a transition period to adopt the new platform, with support and training. After a defined period, the old platform is decommissioned.

**Hard cutover.** A specific date is set for the switch. Communications before the date prepare users; the old platform is read-only or decommissioned on the date itself. More disruptive but resolves the question faster.

The hard cutover works for smaller acquisitions where the user population can be supported through the change in a concentrated period. The phased adoption works for larger acquisitions where the support load of a hard cutover would be unmanageable.

## SharePoint, Drive, and shared content

Shared content migration is consistently the most complex part of email and collaboration handover. The reasons:

The volume is usually larger than people estimate. Years of accumulated documents, decks, spreadsheets, project folders, and team workspaces.

The structure is usually idiosyncratic. The acquired company's information architecture rarely maps cleanly onto the parent's. Decisions about what to migrate, what to archive, and what to discard are not just technical decisions; they affect how people work.

Permissions are usually inconsistent. Many SharePoint and Drive permission structures grow organically over years and reflect the relationships and projects that existed at the time. Migrating them faithfully reproduces the inconsistency in a new environment; redesigning them is a separate piece of organisational work that takes longer than the migration itself.

The pragmatic approach: migrate active content into the new structure, archive inactive content into a clearly labelled archive area in the new tenant, and accept that some content will not be migrated and will be discarded or kept in cold storage. Trying to migrate everything perfectly is the path to a migration project that runs for years.
