# Access and Identity Cutover

## What happens to identity on day one

The honest answer is: as little as possible. Day one is not the day to migrate identity. Day one is the day the parent company gains the legal right to start working on identity migration. The distinction matters.

What does happen on day one: the parent company's identity platform is configured to receive the acquired company's users. Privileged access from the parent side is established for the small number of integration team members who need it. The acquired company's existing identity platform continues to operate. Users at the acquired company log in on day one with the same credentials they used on the day before, into the same systems they used the day before.

What does not happen on day one: bulk user migration. Mailbox migration. SSO consolidation. Forced password changes. Group restructures. Conditional access policy changes affecting acquired users. Any of these on day one creates user-visible disruption with no commercial benefit, because none of them are required for legal completion of the deal.

## The two-tenant period

For most full-absorption integrations involving Microsoft 365 or Google Workspace, there will be a period where two separate tenants exist and users from both need to collaborate. This period typically runs from day one to somewhere between day 30 and day 90, depending on the size and complexity of the acquired estate.

The two main approaches to managing this period:

**Guest access.** The acquired company's users are added as guests to the parent company's tenant, and vice versa. Pros: fast to set up, no account changes for either user population, allows immediate cross-tenant collaboration on shared documents and channels. Cons: guest experience is inferior to full membership, some applications don't handle guests well, and it creates a parallel identity that needs cleaning up later.

**Mail flow and shared address book.** Federated mail flow between the two tenants with a shared global address list, but no guest accounts. Pros: simpler identity model, no parallel accounts. Cons: limited collaboration, often requires running two separate Teams or chat platforms in parallel.

For acquisitions where rapid collaboration matters commercially, guest access is usually the right answer. For acquisitions where the integration is primarily about back-office consolidation and the two businesses operate in different markets, federated mail flow can be sufficient.

## What "identity migration" actually involves

When the migration does happen, usually starting in wave 1 and running across waves 1 and 2, the work is more than a directory sync. The components include:

**Account creation.** New accounts in the parent tenant for each acquired user, provisioned with the right licences, group memberships, and access rights.

**Mailbox migration.** Email content moved from the acquired tenant to the parent tenant, typically using a tenant-to-tenant migration tool. Calendar items, contacts, and shared mailboxes need to be migrated alongside primary mailboxes.

**Endpoint re-enrolment.** Devices that were enrolled in the acquired tenant's MDM need to be re-enrolled in the parent's. For Windows devices joined to the acquired tenant's Entra, this is often the most disruptive part of the migration for the user.

**SSO reconfiguration.** Applications that authenticated against the acquired tenant need to be reconfigured to authenticate against the parent tenant. Each application has its own quirks; budget time for this.

**Conditional access alignment.** The parent's conditional access policies extended to the acquired user population, with carve-outs where necessary for users in countries with specific local requirements.

**MFA registration.** Users registering MFA factors in the parent tenant. This is user-facing work and needs to be communicated and supported.

**OneDrive or Drive migration.** Personal file storage moved between tenants. Easy to underestimate; users have years of accumulated content and the migration tooling can struggle with very large stores.

**Shared content migration.** SharePoint sites, Teams channels, shared drives, and group mailboxes. This is usually the most complex part of the migration and often the part that runs longest.

## Privileged access

Privileged access deserves separate attention because it's the area where day-one mistakes are most expensive. The acquired company's existing administrators retain administrative rights over the acquired tenant on day one. The parent company's administrators do not yet have rights over the acquired tenant unless they've been added during pre-close.

The first technical task in the first hours after close is usually to give the parent company's integration team appropriate administrative access to the acquired tenant. Best practice: named accounts with time-bound, just-in-time elevation rather than permanent global admin grants. Document who got what access and when, both for security and for audit.

The acquired company's existing administrators should retain their rights through the migration period. Removing their access too early leaves the integration team unable to operate the systems users still depend on.

## Country-specific considerations

A few patterns I've seen across European acquisitions:

**Turkey** has data localisation expectations under KVKK. The cleanest approach is usually to keep Turkey-resident users on infrastructure that complies with local data residency requirements, which may mean different conditional access settings or different licence SKUs than the rest of the population.

**Germany** has works council (Betriebsrat) involvement in any system change that affects employee monitoring or data processing. Endpoint management changes, email content scanning, and DLP policies typically require formal works council agreement before deployment to German employees.

**Sweden and the Netherlands** generally have less specific local IT regulation but stronger employee data protection cultures. Migration communications need to be clear about what's being moved and why, more so than in some other markets.

**Portugal** has specific certification requirements for invoicing systems integrated with the tax authority. Identity changes don't usually affect this, but be aware that finance systems may have local certification dependencies.

**The UK post-Brexit** requires UK-EU data transfer arrangements for any cross-border data flows. Identity migration that moves UK user data to EU tenants, or vice versa, needs the appropriate transfer mechanisms in place.

These are constraints to work within, not blockers. But they're constraints that need to be identified during pre-close, not discovered during migration.
