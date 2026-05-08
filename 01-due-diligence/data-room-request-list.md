# Data Room Request List

## How to use this list

This is the list of documents and data points I'd request from a target during IT due diligence. It assumes a typical mid-market acquisition with a few hundred employees and an established IT function. Scale up or down based on the deal size.

The reality of every DD is that you'll get less than you ask for. Submit the full list anyway. What's missing tells you almost as much as what's provided.

## Identity and access

A current export of the directory (Entra, Google Workspace, Okta, or AD) showing all users, account status, and last sign-in date. MFA enforcement policy and current coverage rate. Conditional access policies in force. List of accounts with privileged or administrative rights. Service account inventory with documented purpose and ownership. Joiner, mover, leaver process documentation.

## Application and SaaS

Complete list of business applications with vendor name, primary use case, seat count, contract end date, annual cost, and contract owner. SSO configuration status for each application. Data classification for each application (does it hold customer data, employee data, financial data). Integration map showing which applications are connected to which others.

## Endpoints

Device inventory broken down by operating system and form factor. Management platform deployment status. Encryption coverage. Patch compliance reporting from the last 90 days. Mobile device management arrangements. BYOD policy and current footprint.

## Cloud and infrastructure

List of cloud accounts and tenants across AWS, Azure, GCP, and any other providers. Monthly spend by provider over the last 12 months. Architecture diagrams for any production workloads. List of any on-premise infrastructure with location, purpose, and refresh status. Backup arrangements with frequency, retention, and last successful restore test.

## Network

Office locations with employee count, lease end date, and basic network description. WAN connectivity arrangements. Site-to-site VPN or SD-WAN configurations. ISP and circuit information for each site. Any direct connect or ExpressRoute arrangements with cloud providers.

## Security

Information security policy set. Most recent penetration test report with remediation tracking. Vulnerability management process and current open vulnerability counts by severity. Security awareness training records and phishing simulation results. SIEM or logging arrangements. Endpoint detection and response platform in use. Email security platform and configuration. Cyber insurance policy with coverage limits and claims history.

## Compliance and certifications

Active certifications (ISO 27001, SOC 2, Cyber Essentials, PCI DSS, sector-specific equivalents). Audit reports from the last 24 months. Data protection registration with the relevant supervisory authority. Records of processing activity required under GDPR. Sub-processor list. Any open regulatory matters or supervisory authority engagements.

## Vendor contracts

Master service agreements with the top 10 IT vendors by spend. Microsoft, Google, AWS, or other major platform agreements. Managed service provider contracts with SLA terms. Any contracts with unusual change-of-control, exclusivity, or assignment provisions flagged for legal review.

## People and operations

IT organisation chart with headcount, roles, and reporting lines. Job descriptions for senior IT roles. Salary banding for IT roles, anonymised if necessary. Any consultants, contractors, or interim arrangements currently in place. Documentation of single-points-of-failure where one person holds sole knowledge or access.

## Incidents and operations

Major incident log for the last 24 months with cause, impact, and resolution. Service desk metrics for the last 12 months including ticket volume, response time, and resolution time. Change management records for the last 12 months. Disaster recovery test records.

## Financial

IT operating budget for the current year with variance against last year. IT capital expenditure for the last three years. Vendor spend report for the last 12 months sorted by vendor. Any contractual minimum commitments or unused capacity that might be recoverable as savings.

## Country-specific additions

For acquisitions with operations in regulated jurisdictions, request the local-language documentation rather than translations. Specifically:

For Turkey, KVKK compliance documentation including the data controller registry entry. For Germany, works council agreements affecting IT and any data processing agreements with the Betriebsrat. For Portugal, SAF-T integration documentation and the certification number for any invoicing systems. For the Netherlands, AVG documentation and any agreements with the Autoriteit Persoonsgegevens. For Sweden, IMY notifications and the data protection officer arrangements required under local supplementary law. For the UK post-Brexit, ICO registration and any UK-EU international data transfer arrangements.

These don't need to be reviewed in depth during DD, but their existence or absence is a useful signal of compliance maturity.
