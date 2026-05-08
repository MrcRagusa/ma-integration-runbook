# Integration Runbook Template

## How to use this template

This template is a starting structure for an integration runbook covering a specific acquisition. It's based on the structure I've used across multiple integrations, with confidential content removed and generic sections retained.

The template is deliberately not a fillable form. Different deals need different sections, and a template that tries to anticipate every situation produces runbooks that are simultaneously too long and too generic. Use the structure below as a prompt for what to think about, not as a checklist to complete.

## Suggested structure

### 1. Deal context

Acquiring entity. Acquired entity. Announced date. Expected close date. Deal type (full absorption, platform integration, standalone with shared services, hold separate). Strategic rationale, summarised in two or three sentences. Integration governance, including who owns the integration overall and the IT integration specifically.

This section is reference material. It should be short, factual, and updateable as the deal progresses.

### 2. Scope and approach

What's in scope for IT integration. What's explicitly out of scope. The integration archetype being applied. The chosen identity strategy (full migration, multi-tenant federation, migration with carve-outs, phased migration with parallel running). Any specific commercial or regulatory drivers shaping the approach.

This section is the executive summary. Anyone reading the runbook should be able to understand the integration approach from this section alone.

### 3. Wave plan

A summary of the integration waves, with the work each wave covers, the rough timing, and the named owner for each wave. The wave structure I default to:

Wave 0 (announcement to day one): planning, communication, day-one readiness.

Wave 1 (day one to day 30): identity, communications, support standardisation.

Wave 2 (day 30 to day 90): endpoint management, security baseline, initial application consolidation.

Wave 3 (day 90 to day 180): network and infrastructure, deeper application migration.

Wave 4 (day 180 onwards): application rationalisation at scale, vendor consolidation, longer-term integration.

The wave plan should align to the integration archetype. A hold-separate deal will have a much lighter wave plan than a full-absorption one.

### 4. Workstream detail

For each major workstream, capture:

The current state of the acquired environment.

The target state at the end of integration.

The sequence of work to get from current to target.

The named owner.

The dependencies on other workstreams.

The risks specific to this workstream.

Workstreams to consider: identity, email and collaboration, endpoints, network and infrastructure, security and compliance, applications and SaaS, vendors and procurement, support and service desk.

The depth of detail should match the size of the deal. A small acquisition may have one or two pages per workstream. A large one may have dedicated runbooks for each workstream linked from this top-level document.

### 5. Day-one readiness

A specific checklist of what must be in place before close. The day-one readiness checklist file in this repo provides a starting list. Adapt for the specifics of the deal.

### 6. Risk register

The integration-specific risks, with likelihood, impact, owner, and mitigation. Standard project risks (resource, timeline, scope) belong in the risk register. So do integration-specific risks (key person retention, gun-jumping exposure, data residency, regulatory inheritance) that don't always appear in standard project templates.

### 7. Communication plan

The audiences, channels, and key communication moments. The communication plan template file in this repo provides a starting structure. Adapt for the specifics of the deal.

### 8. Cost and savings tracker

Integration costs by workstream and by category. Savings targets, tracked separately as run-rate (annualised) and realised (banked). Variance against the integration
