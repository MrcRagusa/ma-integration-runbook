# Overview

## What integration is actually about

The phrase "IT integration" gets used loosely. People mean different things by it, and the disagreements usually surface late, after decisions have been made that are hard to reverse.

For the purposes of this runbook, IT integration means three things happening together: bringing the acquired company's people onto the parent company's identity and access systems, bringing their tooling onto the parent company's application estate where consolidation makes sense, and bringing their security and compliance posture up to the parent company's baseline.

Notice what isn't in that definition. Integration isn't about making everything identical. It isn't about migrating every system on a fixed timeline. It isn't about proving that the acquirer's way is better. The point is to reduce risk, capture cost where it's available, and create the conditions for the acquired business to operate effectively as part of the larger group. Sometimes that means full migration. Sometimes it means leaving things alone for two years while more important work happens.

## The five phases

I think about integration in five phases. The folder structure of this repo follows them.

**Due diligence** is the work done before the deal is signed. It's typically rushed, under-resourced, and conducted under NDA. The goal is to surface anything that would change the deal terms, the integration plan, or the integration cost. Most IT due diligence I've seen is too superficial to do this well.

**Pre-close** is the period between announcement and the deal completing. Depending on the regulatory environment, this can be days or many months. It's the planning window. The integration plan that gets locked in during pre-close largely determines whether day one goes smoothly.

**Day one** is the first day the acquisition is legally part of the group. The IT scope on day one is narrower than people expect. It's mostly about communications, support channels, and making sure nothing breaks rather than about migration. The temptation to do too much on day one is consistently the most expensive mistake I see.

**The first 90 days** is when the substantive technical work happens. Identity migrations, license consolidation, network changes, security baseline alignment. The 90-day frame is a useful forcing function but the real work often runs longer.

**The long term** is where most integrations quietly fail. Application rationalisation, vendor consolidation, and the slower work of cultural and process integration. These are the areas that determine whether the acquisition actually delivered the synergies the deal model promised.

## Recurring themes

A few patterns show up across almost every integration I've worked on.

The acquired company's IT estate is always more complex than the data room suggested. Always. Plan for this in the integration cost model rather than treating it as a surprise.

The right integration speed is rarely the fastest possible speed. Speed creates user friction, and user friction during an integration creates retention risk among exactly the people the acquirer wanted to keep. Slower is often cheaper when you account for the second-order effects.

Identity is the longest-running thread. Email cutover gets the attention but the identity work — directory consolidation, group structure, conditional access policies, MFA standards, privileged access — runs for the entire integration and beyond.

Country-level regulatory variation matters more than people expect. A pattern that works for a UK acquisition won't necessarily work for a Turkish or Portuguese one. Data residency, e-invoicing mandates, employment law, and local tax authority requirements all touch IT decisions in ways that aren't obvious from outside the country.

Documentation almost always gets cut when timelines slip. This is a mistake. Every integration creates technical debt, and the difference between manageable debt and unmanageable debt is whether anyone wrote down what was decided and why.

## A note on what's not in this runbook

This isn't a guide to running an integration management office. It isn't a buyer's guide for integration tooling. It isn't legal or tax advice. And it isn't a substitute for senior integration consulting on a complex transaction.

What it is, is a working IT manager's view of what the work actually looks like, written in a form I'd have found useful at the start of my own integration career.
