# Security Baseline Alignment

## What "alignment" means

The acquired company arrives with its own security posture: its own controls, its own tools, its own policies, its own gaps. Bringing that posture up to the parent's baseline is not a single project. It's a structured programme of changes, sequenced by risk, that runs through the first 90 days and often well beyond.

The objective is not to make the acquired environment identical to the parent's. It's to bring the acquired environment to a defensible position relative to the parent's standards, in a sequence that addresses the highest-risk gaps first.

## What to assess in the first 14 days

The first two weeks post-close is when the integration team gains administrative access to the acquired environment. The priority during this period is assessment, not remediation. The aim is to know what's there and what the most acute risks are, so that remediation can be sequenced sensibly.

**Identity and privileged access.** Inventory of administrative accounts, MFA enforcement status, conditional access policies, and any shared or generic accounts. Privileged access gaps are usually the highest-risk findings and need to be addressed first.

**Endpoint posture.** Device management coverage, encryption status, patch posture, and endpoint protection deployment. Devices outside any management framework, or with significant patching gaps, are exposed and represent an immediate risk.

**Email security.** Spam and phishing protection, DMARC/DKIM/SPF posture, and any historical pattern of phishing incidents. Email is the most common initial access vector and weak email security is a frequent finding in mid-market acquisitions.

**Network exposure.** Public-facing services, open ports, exposed administrative interfaces, and any unusual network arrangements. A basic external scan in the first week often reveals exposures the acquired team didn't realise were there.

**Logging and monitoring.** What's being logged, where the logs go, and whether anything is actually monitored. SIEM or equivalent monitoring in the acquired environment is rare in mid-market deals, and integrating the acquired environment into the parent's monitoring is usually a wave 2 priority.

**Backup and recovery.** Whether backups exist, what they cover, where they're stored, and when they were last successfully tested. Untested backups are not backups; they're hypotheses about backups.

**Compliance and certifications.** Certifications held, audit findings outstanding, and any specific regulatory commitments to customers. The integration may inherit compliance obligations that the parent doesn't currently have.

## What to address in the first 30 days

The first month post-close is when the most acute risks get addressed, in roughly this order:

**M
