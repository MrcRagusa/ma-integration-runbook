# Day One Readiness Checklist

## What day one is and isn't

Day one is the first day the acquired company is legally part of the group. It is a milestone, a communication moment, and a logistical exercise. It is not a migration deadline.

The most common and most expensive mistake I see is treating day one as the moment when integration happens. It isn't. Day one is the moment when integration begins. The amount of user-facing change on day one should be the minimum required to make the new corporate structure operational, not the maximum the team can deliver.

Users at the acquired company on day one should be able to do their jobs roughly as they did the day before. The integration work is what changes that over the following weeks and months.

## What must be ready

**Communications.** A welcome message from the parent-company CEO or equivalent, ideally landing on day one. Information about what changes immediately and what doesn't. A clear point of contact for IT questions. Communications about any branding or domain changes that take effect on day one.

**Support channels.** A way for acquired-company users to raise IT issues during the transition. This is often a temporary arrangement: the acquired company's existing helpdesk continues to operate while users are progressively onboarded to the parent's helpdesk over wave 1. A dedicated email alias or Teams channel for transition issues, monitored by both sides' IT teams, works well.

**Identity readiness.** Parent-company identity provider configured with the acquired company as a new domain or organisational unit. Conditional access policies reviewed and adjusted for the new user population. Privileged access arrangements documented. The actual user accounts don't need to exist yet; the platform just needs to be ready to receive them.

**Email continuity.** Acquired-company email continues to flow to acquired-company addresses. No mailbox migrations on day one. If the parent and the acquired entity will eventually share a domain, that's a wave 1 or wave 2 decision, not day one.

**Security minimums.** Parent-company security policies communicated to acquired-company users. Any acute risks (unsupported endpoints, unmanaged admin accounts, exposed services) flagged for immediate attention but not necessarily fixed on day one.

**Procurement and vendor relationships.** A list of acquired-company vendors with contract end dates, ready to start renegotiation or consolidation conversations. Any vendors with change-of-control clauses notified per the contract terms. No actual contract changes on day one.

**Documentation.** A handover pack from the acquired company's IT team or MSP, including credentials, system documentation, and known issues. This often arrives incomplete and gets supplemented in the first week.

## What does not need to be ready

Mailbox migrations. Endpoint re-enrolment. SSO consolidation. Application migrations. Network changes. Data centre exits. Brand changes on shared systems. Any of these can be on the day-one wishlist if the integration is small and the systems are simple, but they shouldn't be on the day-one critical path for a typical mid-market acquisition.

## Stakeholder map for day one

A useful exercise during pre-close is to write down who needs to know what on day one and who's responsible for telling them.

The acquired company's IT team needs to know what's expected of them in the first week and whether their roles continue. This conversation often happens immediately before or on the day itself for legal reasons, so the IT lead on the acquirer side needs to be ready with a clear message.

The acquired company's broader user base needs to know what changes immediately (very little) and where to go for help. Tone matters. The first communication from parent-company IT shouldn't read like a list of policies imposed from outside. It should read like a welcome.

The acquirer's existing IT team needs to know that something has changed and what their part is. This is often where day-one planning falls down: the integration team is fully briefed, the acquired team is being onboarded, and the acquirer's existing service desk hasn't been told anything and starts getting tickets they can't categorise.

External stakeholders, including major vendors, are usually handled through a mix of legal notice and account team conversations. IT is responsible for making sure no critical vendor relationships go silent during the transition.

## A sample day-one timeline

The shape of day one varies by deal but a typical structure looks like this:

In the days immediately before close, the integration team finalises the announcement materials, confirms support channel arrangements, and rehearses the day-one communications. Pre-close gun-jumping rules still apply.

On day one itself, the announcement goes out shortly after legal completion. Users at the acquired company receive a welcome message and basic information. The integration helpdesk goes live. Senior IT leaders on both sides are available throughout the day for escalations.

In the first week post-close, the acquirer's IT team starts the structured handover from the acquired team or MSP. The first batch of acquired users gets onboarded to parent identity, usually starting with senior leadership and the IT team itself. The detailed assessment of the acquired estate begins now that full access is legally permitted.

If day one passes without significant incident, you've succeeded. If it passes with significant migrations actually completed, you've probably done too much and there will be visible friction in the days that follow.
