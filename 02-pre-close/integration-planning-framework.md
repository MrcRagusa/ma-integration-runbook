# Integration Planning Framework

## What pre-close is for

Pre-close is the period between deal announcement and legal completion. Depending on the regulatory environment, the deal size, and any antitrust review required, this can be anywhere from a few weeks to over a year. It is the only window in which you can plan the integration with reasonable information access but without the operational pressure of actually owning the acquired entity.

The integration plan locked in during pre-close largely determines whether day one goes smoothly. Plans that get rewritten in the first week post-close are usually plans that didn't survive contact with the reality of the acquired estate. The aim during pre-close is to do enough work that the day-one plan holds.

## The constraint that shapes everything

Until legal close, the acquirer and the target are still separate companies. Competition law in most jurisdictions prevents detailed operational coordination before close. This is called gun-jumping risk and it's taken seriously by regulators in the UK, EU, US, and most other markets where I've worked.

In practice, this means pre-close integration planning happens through a small group of named individuals on each side, often coordinated through an external clean team or under specific protocols agreed by both sides' legal teams. IT can usually share architectural information and high-level integration plans, but not customer data, pricing, or anything competitively sensitive.

Plan the integration on the assumption that the detailed technical access happens after close, not before. If you build a plan that requires deep knowledge you can only get post-close, you're building a plan that will fail.

## Wave planning

I structure integrations in waves rather than as a single project. The wave structure I've found most useful:

**Wave 0** runs from announcement to day one. It's planning, communication, and the minimum technical work required to make day one functional. No user-visible system migrations happen in wave 0.

**Wave 1** runs from day one to roughly day 30. The focus is identity, communications, and the standardisation of support. Users get parent-company email addresses, get added to the parent's identity provider, and start using the parent's helpdesk channels. The acquired company's existing systems mostly continue to operate as-is.

**Wave 2** runs from day 30 to roughly day 90. The focus is endpoint management, security baseline alignment, and the start of application consolidation where it's straightforward. Devices get enrolled in the parent's MDM platform, the parent's security stack gets deployed, and obvious duplicate SaaS gets rationalised.

**Wave 3** runs from day 90 to roughly day 180. The focus is network and infrastructure consolidation, more complex application migrations, and the substantive work of bringing the acquired entity onto parent-company systems and processes.

**Wave 4** is everything beyond day 180. Application rationalisation at scale, vendor consolidation, and the longer-running work of process and cultural integration.

The wave boundaries aren't sacred. Some workstreams will run faster than the wave they're nominally in, others will run slower. The point of the wave structure is that it creates a shared mental model across the integration team about what's coming when, and it helps prioritise when conflicts emerge.

## Integration archetypes

Not every acquisition needs the same integration approach. The right approach depends on what the acquirer is trying to achieve.

**Full absorption.** The acquired company ceases to exist as a separate entity. Brand disappears, systems consolidate, people move onto parent-company employment terms. This is the most demanding integration archetype and the one that most needs the wave structure above.

**Platform integration.** The acquired company keeps its brand and customer-facing identity but moves onto the parent's back-office platforms (finance, HR, IT). Common in PE-backed buy-and-build strategies. Lighter on user-facing change but still requires substantial integration work behind the scenes.

**Standalone with shared services.** The acquired company operates largely independently but shares specific services with the parent (often security, identity, and procurement). Lighter integration work but creates ongoing complexity in how shared services are governed.

**Hold separate.** The acquired company is run as a portfolio investment with no operational integration. IT has minimal work to do beyond ensuring basic security and reporting. Rare outside specific PE structures.

The integration archetype is a deal-team decision, not an IT decision. But the IT plan needs to match the archetype. A full-absorption plan layered onto a hold-separate deal will create friction and waste, and a standalone plan layered onto a full-absorption deal will leave the integration unfinished.

## What good pre-close output looks like

A one-page integration approach summary that the deal team and acquired-company leadership can both understand. A detailed wave plan with named owners and rough timing. A day-one readiness checklist (see the separate file). A risk register that covers both technical risks and integration-specific risks like key person retention and gun-jumping exposure. A communication plan covering announcement, day one, and the first 30 days.

What you don't need pre-close: detailed migration runbooks, finalised tooling decisions, or a perfect view of the acquired estate. Those are wave 1 and wave 2 work.
