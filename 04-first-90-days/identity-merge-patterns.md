# Identity Merge Patterns

## Why identity is the longest thread

Mailbox migration finishes. Endpoint re-enrolment finishes. Network changes get cut over and the project closes. Identity work, almost uniquely, doesn't really finish. Directory consolidation, group structure rationalisation, conditional access alignment, and the long tail of orphaned accounts and stale permissions runs for the entire integration and well beyond.

This is also the area where shortcuts taken in wave 1 create problems that surface six, twelve, or eighteen months later. A directory that was merged hastily, a group structure that was preserved unchanged from the acquired tenant, or conditional access policies that carved out the acquired population permanently rather than temporarily — these create operational debt that's expensive to repay later.

Worth investing the time during the first 90 days to get the foundations right, even if it means accepting a slower pace of visible progress.

## The four patterns

Across the integrations I've worked on, four broad patterns recur for handling identity in the first 90 days.

**Full migration.** The acquired company's directory is fully migrated into the parent's, the acquired tenant is decommissioned, and the acquired population becomes operationally indistinguishable from the rest of the parent's user base. This is the right answer for full-absorption integrations where the acquired entity will not retain a separate identity.

**Multi-tenant federation.** The acquired tenant remains operational but is federated with the parent for SSO, shared identity, and cross-tenant collaboration. Used where there are specific reasons to maintain a separate tenant, including data residency requirements, specific regulatory constraints, or a deliberate hold-separate strategy.

**Migration with carve-outs.** The bulk of the acquired population is migrated to the parent tenant, but a subset remains in a separate identity arrangement. Common where most of the workforce can be fully integrated but a specific country, function, or regulated entity needs to remain distinct.

**Phased migration with parallel running.** The acquired tenant is kept operational while users are progressively migrated to the parent. Both directories work in parallel for a period, with eventual decommissioning of the acquired tenant once migration is complete. This is the most common pattern for medium and large acquisitions, because it allows the migration to be sequenced rather than executed as a single high-risk cutover.

The pattern decision should be made during pre-close planning and confirmed in the first weeks post-close, once the integration team has detailed access to the acquired estate.

## Sequencing the migration

Within a phased migration, the sequencing of users and groups affects how smoothly the work progresses. The pattern I've found works best:

**Wave 1.1: Integration team and pilot users.** The IT team itself migrates first, plus a small group of senior leaders who have volunteered to be early adopters. This is the testing wave. Mistakes get made on people who can absorb them.

**Wave 1.2: Service accounts and shared resources.** Service accounts, shared mailboxes, distribution lists, and Microsoft 365 groups. Less user-visible but technically significant; getting these wrong creates persistent operational issues.

**Wave 2.1: Functional teams without external dependencies.** Teams whose work is mostly internal to the acquired entity. Less risk of disrupting external relationships if something goes wrong.

**Wave 2.2: Customer-facing and partner-facing teams.** Sales, customer success, account management, and any other roles where mailbox issues or calendar issues directly affect external relationships. Migrate these only after the earlier waves have been validated.

**Wave 3: The long tail.** Contractors, infrequent users, dormant accounts that are still active for legitimate reasons. Often more complex per-user than the bulk migration because each one has specific quirks.

Resist the temptation to migrate by office or country. Office-based migration is administratively convenient but it creates a period where teams whose members work across offices are split between two directories, with collaboration friction throughout. Function-based migration keeps collaborative teams together through the transition.

## Group structure decisions

The acquired company arrives with its own group structure: distribution lists, Microsoft 365 groups, security groups, and Teams. Decisions need to be made for each:

**Migrate as-is.** The group continues to exist in the parent tenant with the same membership and purpose. Right answer for groups that represent durable organisational structures.

**Migrate and rename.** The group is preserved but renamed to fit the parent's naming conventions. Right answer for groups whose purpose is durable but whose naming reflects acquired-company conventions that won't survive integration.

**Merge with existing parent group.** The acquired group's membership is merged into an existing parent-company group. Right answer where the same function exists in both organisations and there's no reason to maintain separation.

**Decommission.** The group is not migrated and is allowed to fall away. Right answer for groups that were specific to the acquired company's structure and have no equivalent purpose in the parent.

This work is tedious but worth doing carefully. Migrating groups uncritically creates a directory full of duplicates and obsolete artefacts that become permanent unless deliberately cleaned up.

## Conditional access alignment

The parent's conditional access policies need to extend to the acquired user population, but the timing matters. Apply parent policies too early, before users have completed identity migration, and you lock people out. Apply them too late, and you operate with an unprotected user population for longer than necessary.

The pattern I've used: extend the parent's conditional access policies to acquired users in two phases. First, a baseline set of policies that match the acquired company's existing protections, applied immediately on identity migration. Second, the parent's full policy set, applied once the user has had time to register MFA factors, configure devices, and adapt to the new environment.

Country-specific carve-outs deserve explicit treatment rather than implicit drift. A policy exception for a Turkey-based user population because of KVKK requirements is legitimate. The same exception left in place a year later because nobody removed it is operational debt.

## What to clean up before declaring done

Before considering the identity migration complete, the following are worth checking:

Service accounts in both the source and destination directories are inventoried and either migrated or formally retired. Orphaned service accounts are a common source of later security findings.

Permissions on shared content reflect the new identity structure rather than the old one. Migrated permissions that reference the source tenant create access issues that surface unpredictably.

Privileged access in the destination tenant follows the parent's standards: named accounts, time-bound elevation, MFA enforced. Permanent global admin grants that were created during the integration urgency get forgotten and become audit findings.

The source tenant, once decommissioned, is properly closed: licences released, data exported as required for retention, contracts cancelled. Tenants left in a partially-decommissioned state continue to incur cost and create confusion.
