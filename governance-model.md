# Knowledge Governance Model: High-Growth SaaS Pattern

This document generalizes the governance model recommended in the [case study](README.md) engagement. It shows the structural patterns: space architecture, metadata schema, content lifecycle, and the KPI framework used to measure progress. Client-specific tooling and identifying details are omitted.

---

## Space Architecture

A tiered structure separates content by audience and AI ingestion scope. Mixing employee-facing self-service content with internal specialist procedures in the same space is a common cause of the discovery gap: search returns too much irrelevant material, and AI assistants ingest content never meant for end users.

| Space Type | Purpose | Access | AI Ingestion |
|-----------|---------|--------|---------------|
| Self-Service | Employee-facing articles: how-to guides, FAQs, common request procedures | All employees and contractors | Yes |
| Runbooks | Technical procedures for specialists: provisioning, troubleshooting, configuration | Specialist team only | No |
| Governance | Access matrix, policies, SOPs, review schedules, compliance documentation | Function team and Compliance | No |
| Department spaces | Non-IT departmental content, governed but not centrally owned | Defined per department | Selective |
| Archive | Retired content from all spaces, searchable for historical reference | Function team | No |

Personal, ungoverned spaces are deprecated. Existing ones with valuable content are migrated into the appropriate governed space; the rest are archived.

---

## Required Metadata

Every article carries the following properties. This is the same governance principle applied across engagements: machine-readable by default, so that human navigation and AI agent queries are served by the same fields.

| Property | Purpose |
|----------|---------|
| Title | Follows a naming convention: [Category] - [Description] |
| Status | Draft, In Review, Published, or Archived |
| Owner | Named individual responsible for content accuracy |
| Content Type | Article, Runbook, FAQ, SOP, or Onboarding Guide |
| Last Reviewed | Date someone last verified the content is current |
| Created By | Original author, for traceability |
| Audience | All Employees, Internal Team, Contractors, or a Specific Role |

---

## Content Lifecycle

The same four-stage pipeline used across knowledge governance engagements: content enters as a Draft, moves through review, earns Published status, and is retired to Archived when no longer current.

| Status | Definition | Reader Signal |
|--------|-----------|---------------|
| Draft | Being written or incomplete. Not yet reviewed for accuracy. | Do not rely on this for decisions. |
| In Review | Complete and submitted for review. The author considers it ready. | Treat as provisional. |
| Published | Reviewed, approved, and the current authoritative version. | Safe to rely on. |
| Archived | Outdated or superseded. Retained for historical traceability. | Historical reference only. Check for a replacement link. |

**Lifecycle rules:**
- Content is archived, never deleted. This preserves the audit trail and protects institutional memory.
- Published content not reviewed in 90 days is flagged for the content owner during the monthly review cycle.
- Significant revisions to Published content create a new Draft; the original is archived with a cross-reference.

---

## Contractor Access Matrix

A documented framework closes a common compliance gap: ad hoc, undocumented access decisions that an auditor cannot verify.

| Space Type | Contractor Access | Approval Required |
|-----------|-------------------|--------------------|
| Self-Service | Yes (default) | No |
| Runbooks | No | Exception approval required |
| Governance | No | No exceptions |
| Department spaces | Defined per department | Department owner approves |
| Archive | No | No exceptions |

The matrix is documented, referenced in onboarding and offboarding checklists, and reviewed quarterly. Access is provisioned through identity management groups mapped to space permissions, not granted case by case.

---

## Review Cadence

| Review Type | Frequency | Responsibility |
|-------------|-----------|----------------|
| Article freshness review | Monthly | Content owner reviews own articles flagged as 90+ days since last review |
| Space health check | Quarterly | Knowledge management function reviews space structure, orphan pages, permission accuracy |
| AI assistant performance review | Monthly | Function reviews deflection rate, unanswered query categories |
| Compliance review | Quarterly | Function and Compliance jointly review access matrix and archival records |

---

## Governance as Compliance Infrastructure

A governed knowledge base produces compliance evidence as a by-product of normal operation, rather than as a separate audit-preparation exercise.

| Control | How Governance Provides It |
|---------|----------------------------|
| Access control documentation | Contractor access matrix: defined, documented, quarterly reviewed |
| Procedure documentation | SOPs and runbooks: documented with ownership, review dates, version history |
| Audit trail | No-deletion policy. Archived content retained with full version history. |
| Evidence of ongoing compliance | Monthly review cadence, quarterly health checks, documented review dates on every article |

---

## Success Measurement

Three tiers of KPIs separate whether the work is happening, whether it is producing early traction, and whether it is solving the underlying problem.

### Activity KPIs: Is the work happening?

| KPI | How to Measure | Target |
|-----|----------------|--------|
| Articles published | Count of Published articles in governed spaces | Defined per content roadmap |
| Metadata completeness | Articles with all required fields populated | 100% of new articles |
| Naming convention compliance | Articles following the standard pattern | 90%+ |
| Review cadence adherence | Monthly freshness reviews completed on schedule | 100% |

### Leading KPIs: Is there early traction?

| KPI | How to Measure | Target |
|-----|----------------|--------|
| Ticket deflection rate | Ticket volume in documented categories vs. pre-documentation baseline | 15-25% reduction in documented categories |
| AI assistant resolution rate | Percentage of queries resolved without human intervention | Improvement over baseline |
| Content freshness | Published articles where Last Reviewed is older than 90 days | Zero stale Published articles |

### Outcome KPIs: Is the underlying problem solved?

| KPI | How to Measure | Target |
|-----|----------------|--------|
| Employee self-service satisfaction | Short survey administered periodically: Can you find answers? Do you trust the content? | 75%+ positive responses as baseline |
| Follow-the-sun coverage | Ticket volume from non-primary-business-hours offices, for categories with published content | Measurable reduction vs. baseline |

---

*This document generalizes a governance model produced as part of a strategic advisory engagement by [Coreso Collaborative](https://coresocollaborative.com). Client-identifying details have been removed. The full engagement is described in the [case study](README.md).*
