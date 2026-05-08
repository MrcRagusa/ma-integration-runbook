# Red Flags and Deal Breakers

## The distinction

A red flag is something that increases integration cost or risk and needs to be priced into the deal. A deal breaker is something that should stop the transaction or fundamentally change its structure. Most red flags are not deal breakers, but some are, and IT DD is occasionally where they get found.

The list below is drawn from patterns I've seen repeatedly across acquisitions in the UK, Netherlands, Sweden, Germany, Portugal, and Turkey. Country-specific patterns are noted where relevant.

## Red flags that are usually manageable

**No formal IT function.** Common in companies under about 50 people. Means there's no one to interview, no documentation, and no clear ownership. Adds time to the integration but rarely changes the deal.

**Heavy reliance on a single MSP.** Particularly common in smaller acquisitions in continental Europe. The MSP often holds the only credentials, the only documentation, and the only operational knowledge of the estate. Plan for an MSP transition or replacement on day one and budget accordingly.

**Outdated endpoint estate.** Old hardware, unsupported operating systems, no central management. Costly to remediate but well understood. Get a refresh budget into the integration plan.

**Shadow IT sprawl.** Departments running their own SaaS subscriptions outside finance and IT visibility. The cost of consolidation is usually less than the licence savings, so it pays for itself, but it takes time to discover what's actually in use.

**No formal information security function.** Common below a certain scale. Manageable through the integration if the parent has a mature security team that can absorb the work.

## Red flags that materially change the integration

**Tenant or directory complexity.** Multiple Microsoft 365 tenants, fragmented Active Directory forests, or a mix of Google Workspace and Microsoft 365. The directory consolidation work alone can run six to twelve months and significantly increases day-one complexity. Make sure this is reflected in the integration cost.

**Significant on-premise infrastructure.** Particularly if it's hosting customer-facing or production systems. The decision to migrate, lift-and-shift, or maintain becomes a major workstream in its own right.

**Unusual contract terms.** Change-of-control clauses that void key contracts, exclusivity arrangements that prevent consolidation with the acquirer's vendors, or auto-renewal clauses with long notice periods. These need to be flagged to legal during DD, not discovered after close.

**Country-specific data residency requirements.** Turkey's KVKK requires certain personal data to be stored in Turkey. Germany has historical sensitivities around cross-border data transfer that affect cloud migration planning. Both can be managed but they constrain integration choices and should be priced in.

**E-invoicing or local tax authority integrations.** Portugal's SAF-T and Italy's SDI requirements mean that finance systems are tightly coupled to local tax infrastructure. Migrating or replacing those systems isn't impossible but it's a regulated workstream rather than a standard IT project.

## Patterns that should prompt a deeper look

**Reluctance to share information during DD.** Sometimes legitimate (genuine confidentiality concerns, busy team, tight DD timeline). Sometimes a signal that there's something the seller doesn't want surfaced. Push harder rather than accepting silence.

**A founder or owner who personally administers core systems.** They often hold credentials, knowledge, and access patterns that have never been documented. Plan a structured handover during the transition or you'll lose institutional knowledge that's hard to recover.

**Unusual cloud cost patterns.** Either much higher or much lower than expected for the company size. High suggests waste or undiscovered workloads. Low can suggest unmaintained legacy infrastructure or under-investment that will need correcting.

**Recent senior IT departures.** People leaving just before or just after a deal announcement is a signal worth investigating. They may know something about the estate that hasn't surfaced in DD.

## Genuine deal breakers

These are rare but they happen. They should be escalated to the deal lead immediately.

**Active or recent security incident.** A breach in progress, an unresolved ransomware event, or evidence of ongoing compromise. The transaction may need to pause, the deal terms may need to change to allocate liability, and disclosure obligations to regulators or customers may be triggered.

**Material misrepresentation in the data room.** If the data room states one thing and the technical reality is materially different in a way that affects valuation, that's a finding for the lawyers, not just for IT.

**Regulatory non-compliance with deal-relevant frameworks.** GDPR violations of significant scale, missing certifications that customer contracts require, or operations in regulated sectors without the required permissions. These don't always stop deals but they always change them.

**Critical system dependencies on people who will leave.** If the only person who understands a customer-facing production system is the founder, and the founder is exiting at close, that's a deal-breaker-adjacent issue that needs an explicit transition plan as a condition of closing.
