# Network and Infrastructure Merge

## The work that's mostly invisible

Network and infrastructure integration is the work users notice least when it goes well and most when it goes badly. The objective is to bring the acquired company's network, connectivity, and underlying infrastructure into a state where it operates as part of the parent's environment, with consistent security posture, manageable cost, and no user-facing surprises.

Most of this work happens between day 30 and day 180. It's rarely on the critical path of the integration in commercial terms, but it consumes a meaningful share of the IT integration budget and creates risk if rushed or deferred.

## What to inventory in the first 30 days

The data room view of network and infrastructure is almost always incomplete. The first 30 days post-close is when the integration team can build an accurate picture.

**Office connectivity.** For each acquired site: ISP, circuit type, bandwidth, contract end date, current cost, and any dependencies (such as shared infrastructure with neighbouring tenants in serviced offices). Fibre and dedicated lines look very different in cost terms from cable broadband or business-grade consumer connections.

**WAN architecture.** Site-to-site VPNs, MPLS arrangements, SD-WAN deployments, or direct connect/ExpressRoute links to cloud providers. The architecture diagrams in the data room are often outdated; verify against current state.

**Wireless infrastructure.** Access points, controllers, authentication arrangements, and guest network configurations. Wireless is often the most user-visible component of network integration because acquired users will be expecting their devices to connect to the new network seamlessly.

**Voice and contact centre.** Phone systems, contact centre platforms, and any specialised telephony arrangements. Often run by a separate team or vendor and easy to miss in IT-led inventories.

**Cloud workloads.** AWS, Azure, GCP, or other cloud accounts with the workloads they host, the people with access, and the monthly spend. Pay particular attention to test, dev, and abandoned environments that may have been forgotten by the acquired team.

**On-premise infrastructure.** Any servers, storage, or specialist equipment in offices, data centres, or co-location facilities. Note the refresh status and contract arrangements separately from the network inventory.

**Internet-facing services.** Public DNS records, websites, customer-facing applications, and any other services exposed to the internet. Worth doing a basic external scan to validate against the documented inventory.

## Decisions to make during the first 60 days

**Office network strategy.** For each acquired office, decide whether to bring it onto the parent's standard network architecture, leave it operating independently, or close it. The decision depends on the parent's existing approach: companies with strong central network architecture usually integrate offices fully; companies that operate offices independently may leave the acquired sites largely as they are.

**WAN approach.** Whether to extend the parent's WAN to the acquired sites, replace the acquired company's WAN entirely, or maintain separate connectivity. SD-WAN architectures generally make extension easier than traditional MPLS-based ones.

**Cloud account strategy.** Whether to migrate acquired cloud workloads into the parent's cloud accounts, leave them in their existing accounts under parent governance, or run a deliberate multi-account architecture. The choice depends on workload characteristics and on the parent's existing cloud governance maturity.

**Data centre and on-premise.** Whether to migrate any on-premise workloads to cloud, consolidate them into the parent's data centre, or leave them in place. Lift-and-shift to cloud is often the right answer for workloads that have been quietly running on aging hardware; in-place modernisation is rarely worth the effort during integration unless there's a specific business reason.

## Common patterns and pitfalls

**Hub-and-spoke or mesh decisions.** When extending the parent's WAN to acquired sites, the topology choice has implications for cost, latency, and resilience. Hub-and-spoke is simpler but creates a single point of failure at the hub. Mesh architectures are more resilient but more expensive and more complex to operate. Most integrations land somewhere between, with primary hub connectivity and selective mesh links for specific high-traffic patterns.

**Shadow connectivity.** The acquired company often has connectivity arrangements that aren't documented and weren't surfaced during DD. A specific risk: site-to-site VPNs to former parent companies (where the acquired entity was itself once part of a larger group), to specific customers, or to development partners. These need to be discovered, documented, and either retained deliberately or decommissioned.

**Cloud account sprawl.** Acquired engineering teams sometimes have multiple AWS or Azure accounts that have grown organically. Consolidation into the parent's account structure is usually the right answer but can disrupt running workloads if mishandled. Plan the migration carefully and use cloud-native tooling for cross-account moves where possible.

**On-premise hardware refresh timing.** Acquired companies sometimes have on-premise hardware that's near end-of-life and was being deferred until after the deal. The deferred refresh becomes the integration team's problem post-close. Identify these situations during discovery and budget for either replacement or migration.

**Voice and telephony complexity.** Phone systems are often more integrated with business processes than people realise: call recording for compliance, call routing for customer support, hunt groups for sales. Migrating telephony usually requires more planning than the technical complexity alone suggests.

**Internet-facing services and DNS.** Domain transitions create user-facing visibility. Customer-facing websites, marketing domains, and email domains all need careful sequencing. DNS changes that look simple often have downstream effects on email deliverability, SSL certificates, and any third-party integrations that whitelist specific hostnames.

## Country-specific considerations

Network and infrastructure integration interacts with country-specific factors in a few specific ways:

**Data residency.** Cloud workload migration plans need to account for any data that must remain in a specific jurisdiction. The right pattern is usually to keep regulated data in-country and migrate the supporting infrastructure around it, rather than trying to move the data.

**Local connectivity.** Connectivity options vary significantly by country. Fibre availability, business broadband markets, and the maturity of SD-WAN providers all differ. Solutions that work in the UK or the Netherlands may not be available, or may be much more expensive, in markets with less developed connectivity infrastructure.

**Telecoms regulation.** Voice and telephony are regulated separately from data services in most jurisdictions. Cross-border voice arrangements need to comply with local telecoms law, and certain services that are unregulated in one country may require local licences in another.

**Site-specific arrangements.** Offices in some markets come with infrastructure that's tied to the building or to specific landlord arrangements. Internet connectivity in serviced offices, in particular, can be opaque and difficult to change. Identify these constraints during discovery.

## When to declare done

Network and infrastructure integration rarely has a clean completion date. The work tapers rather than ends. Useful milestones to mark progress:

The acquired sites are operating on the parent's standard network architecture, or are operating independently under a documented and deliberate decision to do so.

The acquired cloud workloads are operating in the parent's cloud governance framework, with appropriate access controls, cost monitoring, and security posture.

The acquired company's infrastructure no longer requires specialist knowledge held only by acquired-company staff. Either the knowledge has been transferred to the parent's team, or the systems requiring that knowledge have been retired or replaced.

The infrastructure inventory is current and matches the operational reality. This last one matters more than it sounds: the inventory is the basis for security, compliance, and cost management, and an outdated inventory undermines all three.
