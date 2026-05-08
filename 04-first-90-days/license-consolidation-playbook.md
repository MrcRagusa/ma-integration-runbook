# Licence Consolidation Playbook

## The opportunity

Most acquisitions inherit overlapping software licences. The same productivity suite, the same security tools, the same project management software, the same design tools. The combined entity rarely needs both sets, and consolidation typically generates meaningful savings without affecting end-user functionality.

In one integration programme I was responsible for at Sovos, structured licence consolidation across the acquired estate generated approximately £127,000 in annual savings. That figure is achievable in many integrations of similar scale, but only if the work is approached systematically and started early. Licence consolidation that gets pushed past the first renewal cycle of the acquired company's contracts captures significantly less value, because the renewal terms lock in spend that's harder to unwind.

## The first 30 days: discovery

The acquired company's licence position is rarely accurately represented in the data room or in the finance system's vendor records. Discovering the actual position is the first task.

Sources to combine:

The acquired company's finance records of vendor spend over the last 12 months. Filter for software and SaaS vendors. This catches contracted spend but misses anything billed to corporate cards or expense claims.

The acquired company's SSO provider's application catalogue. Anything users sign into via SSO appears here, even if it isn't recognised as a corporate purchase.

The acquired company's identity provider's enterprise application list. Sometimes broader than the SSO catalogue, particularly in environments where SSO adoption is incomplete.

The acquired company's expense data, filtered for software vendors. This catches the shadow IT that doesn't appear in the formal procurement records.

Direct conversations with department heads, particularly in functions that tend to have their own software stacks: marketing, design, engineering, sales, and finance. Often surfaces tools that don't appear in any of the systematic sources.

Combine the sources and reconcile the differences. Expect the discovered footprint to be 20 to 50 percent larger than the data room indicated.

## The first 60 days: rationalisation decisions

For each application discovered, a decision is needed:

**Retain at the parent's standard.** The acquired company's tool will be replaced by the parent's existing equivalent. Users migrate; acquired-company contract gets cancelled or not renewed.

**Retain at the acquired company's standard.** The parent's existing tool will be replaced by, or supplemented by, the acquired company's equivalent. Less common but happens where the acquired company has a clearly superior tool.

**Retain both.** Both tools continue to exist for legitimate reasons, usually because they serve different use cases or different user populations.

**Cancel both.** Rare but happens when neither tool is actually required and the consolidated entity can do without.

The decision is sometimes obvious (the parent's enterprise Microsoft 365 agreement clearly continues; the acquired company's standalone Microsoft 365 agreement gets terminated). It's often less obvious where both companies have made deliberate choices that suit their existing operations.

A practical decision framework: prefer the tool that serves the larger user population, has lower per-user cost at the combined scale, and has a contract structure that allows flexible scaling. Where these point in different directions, default to the parent's tool unless there's a specific reason not to.

## The first 90 days: execution

Cancellation and consolidation actions need to be executed during the contract notice windows, not after. Most SaaS contracts have notice periods of 30, 60, or 90 days for non-renewal. Missing the notice window often locks in another full year of spend.

For each tool being consolidated:

Confirm the contract notice period and the next renewal date. Calendar the action date.

Plan the user transition. If users are moving from tool A to tool B, they need access to tool B, training where appropriate, and a date by which tool A will become unavailable. Don't cancel tool A before users have transitioned, but don't leave the transition open indefinitely either.

Export any data from tool A that needs to be retained. Some tools make this easy; some make it deliberately difficult. Build the export work into the migration plan.

Issue the cancellation notice in writing per the contract terms. Verbal arrangements with account managers don't count if there's a dispute later.

Confirm the cancellation has been processed, the final invoice has been received, and any auto-renewal has been disabled. Vendors occasionally fail to process cancellations correctly, particularly during the period leading up to a renewal date.

## Specific patterns to watch for

**Microsoft 365 licence overlap.** The single largest consolidation opportunity in most integrations. Combining acquired-company users into the parent's Microsoft 365 enterprise agreement usually unlocks significant per-user discounts. Plan the timing carefully because adding users mid-term has different commercial implications than adding them at renewal.

**Security tool stack.** Both companies typically have endpoint protection, email security, and SIEM-type tools. Consolidating to a single stack reduces cost and simplifies operations. The decision is usually driven by which stack the parent's security team is committed to operating long-term.

**Productivity and collaboration overlap.** Where one company uses Microsoft 365 and the other uses Google Workspace, full migration to one platform is normally the right answer for full-absorption integrations. The licence consolidation savings are large; the user-disruption costs are also large. Plan accordingly.

**Adobe and creative tool overlap.** Smaller in dollar terms but technically tricky because Adobe's licensing structure and team management has its own quirks. Worth involving an Adobe specialist if the combined estate is larger than a few dozen seats.

**Project management and collaboration tools.** Asana, Monday, Jira, Trello, ClickUp, and similar tools often exist in multiple variants across acquired companies. Consolidation is straightforward in licence terms but harder in user-experience terms because teams have built workflows around their preferred tool. Don't underestimate the change management work.

**Shadow tools that don't appear in formal procurement.** Particularly in marketing, design, and engineering. Often individually small but cumulatively significant. Set a threshold below which consolidation isn't worth chasing, and apply it consistently.

## Reporting the savings

For the integration to get credit for licence consolidation savings, the savings need to be visible to finance and to the deal team. A simple format:

For each consolidation action, capture: tool, action taken, date of action, annual cost previously, annual cost now, and net annual saving. Aggregate to a programme total.

Report the total savings monthly during the first 90 days, then quarterly thereafter. Show both run-rate savings (annualised) and realised savings (actually banked). The two figures diverge during the first year and converge after that.

Avoid claiming savings that are actually cost avoidance. If the parent was about to renew a contract anyway, declining to renew it because of consolidation is a legitimate saving. If the parent had no plans to renew anyway, claiming the saving inflates the number and reduces the credibility of the reporting.
