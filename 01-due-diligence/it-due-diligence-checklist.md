# IT Due Diligence Checklist

## What due diligence is for

IT due diligence has three jobs: surface anything that would change the deal terms, surface anything that would change the integration plan, and surface anything that would change the integration cost. If a piece of information doesn't change one of those three things, it doesn't belong in the IT DD report.

That framing matters because IT DD is almost always rushed, conducted under NDA with limited access to the target's systems, and competing with commercial, financial, legal, and HR workstreams for the same handful of available hours with the target's leadership. Triage is the entire job.

## What to ask for

The data room rarely contains what you actually need. Expect to submit specific information requests and follow up multiple times. The list below is what I'd ask for on every IT DD, regardless of deal size or geography.

**Identity and access**

Total user count, broken down by employee, contractor, and service account. Identity provider in use (Microsoft Entra, Google Workspace, Okta, on-prem Active Directory, or some hybrid). MFA coverage and enforcement policies. Privileged access arrangements, including how many people hold global admin or equivalent rights and how those accounts are protected. Any shared or generic accounts still in use.

**Application estate**

A full list of SaaS applications with seat counts, contract end dates, and annual cost. The list will always be incomplete. Cross-reference with the finance team's expense data and with the SSO provider's application catalogue to find shadow IT.

**Endpoints**

Device count by type (Windows, macOS, mobile). Management platform in use (Intune, Jamf, Kandji, Workspace ONE, or none). Encryption coverage. Patch posture. Any BYOD arrangements.

**Network and infrastructure**

Office locations and lease end dates. Network topology, including any site-to-site VPNs, MPLS links, or SD-WAN deployments. Cloud hosting providers and approximate spend. Any on-prem servers or data centre presence. Backup and disaster recovery arrangements.

**Security and compliance**

Certifications held (ISO 27001, SOC 2, Cyber Essentials, sector-specific equivalents). Last penetration test date and remediation status. Known incidents in the last 24 months. Cyber insurance coverage and any open claims. Data protection arrangements, including DPO appointment status if operating in the EU or UK.

**Vendors and contracts**

Top 10 IT vendors by spend, with contract end dates and any auto-renewal clauses. Any vendors with unusual exclusivity, change-of-control, or assignment clauses. Particular attention to the Microsoft, Google, Adobe, AWS, and managed service provider relationships, which tend to be the largest and most operationally critical.

**People and capability**

IT team headcount and roles. Reporting line. Any single points of failure (the classic "if person X leaves, we can't operate system Y" risk). External dependencies on contractors or MSPs.

## How to score what you find

I prefer a simple traffic light against integration cost and integration risk for each area, rather than a complex maturity model. The audience for the IT DD report is usually the deal team, not other IT people, and they need clarity about what changes and what doesn't.

Green means the area is broadly aligned with the acquirer's standards and integration will be straightforward. Amber means there's meaningful work to do but it's well understood and the cost can be estimated. Red means either there's a problem that affects the deal directly, or the information available isn't sufficient to assess the area properly. Reds need to be flagged to the deal lead immediately rather than waiting for the report.

## What good DD output looks like

A short executive summary aimed at the deal team, listing the top three risks and the integration cost estimate. A detailed appendix aimed at whoever runs the integration, with section-by-section findings. A list of follow-up questions that didn't get answered before the deal closed, to be revisited on day one or shortly after.

Avoid the temptation to write a long, comprehensive report. The deal team won't read it. The integration team needs the answers, not the working.
