# Application Rationalisation

## Why this is where most integrations fail

The most common failure mode I've seen in IT integration is not technical. It's that the integration stops at "everyone has email and can log in" and never actually rationalises the application estate. The acquired company's tools continue to operate alongside the parent's, contracts get renewed without scrutiny, and the integration synergies that were promised in the deal model never appear in the operating budget.

This happens because application rationalisation is harder than mailbox migration. It involves business stakeholders, not just IT. It surfaces disagreements about how work gets done, not just where data lives. And it runs over months and years rather than weeks, which means it competes with whatever fresh priorities have arrived since the integration was new.

Treating application rationalisation as a structured programme rather than as a tail of integration work is the difference between an integration that delivers its synergies and one that quietly doesn't.

## What rationalisation actually means

The phrase gets used loosely. For practical purposes, application rationalisation means deciding for each business application whether the consolidated entity will use the parent's version, the acquired company's version, both, or neither. And then actually executing the decisions, which is where the work lives.

The decision points usually break into four categories:

**Productivity and collaboration.** Office suite, email, chat, video conferencing, file storage. Usually consolidated early in the integration as part of identity and email migration. Application rationalisation here is largely already done by day 90.

**Back-office systems.** Finance, HR, payroll, procurement. These are typically consolidated as part of the broader business integration rather than as IT-led projects, but IT is responsible for the technical execution. Timelines run from six months to multiple years depending on system complexity.

**Function-specific systems.** Sales tools (CRM, sales engagement, contract management), marketing tools (marketing automation, content management, analytics), engineering tools (development platforms, observability, project management), customer support tools, and so on. This is the largest category and usually the messiest, because each function has its own preferences and switching costs.

**Customer-facing systems.** Anything that customers interact with directly. Usually rationalised last, if at all, because the cost of changing customer-facing systems often exceeds the savings from consolidation.

Different categories need different approaches.

## A framework for the function-specific category

Function-specific applications are where I've seen the most variation in how integrations are handled, and where structure matters most.

For each application area (CRM, marketing automation, project management, and so on), the integration team needs to capture:

What tools each company uses today, and at what scale.

What the contract terms are, including renewal dates and exit costs.

What the user populations look like, including any specialist users (administrators, integrators, power users) whose change costs are higher than typical.

What integrations exist with other systems, and what would break if the tool were retired.

Then, for each tool area, a decision is made: standardise on the parent's, standardise on the acquired company's, run both with clear scope boundaries, or replace both with a third option. The default decision should be "standardise on the parent's tool" unless there's a specific reason not to. Defaults that get overridden too easily lead to integrations
