# Knowledge Management Strategy for a High-Growth SaaS Company

An AI assistant can only resolve what is properly documented. When internal knowledge has no governance, no ownership, and no lifecycle, the AI built on top of it inherits the same gaps: it cannot tell current content from outdated content, and it cannot surface knowledge that was never captured in the first place. This case study documents a strategic advisory engagement that treated AI assistant underperformance as a content governance problem, not a tool configuration problem.

## What This Repository Contains

- **This file:** the case study narrative: problem, approach, strategy, and key design decisions.
- **[Governance Model](governance-model.md):** the structural patterns: space architecture, metadata schema, content lifecycle, and the KPI framework used to measure progress. Generalized from the engagement's recommendations.

---

## Client

A Canadian SaaS company in the technology sector. The organization had more than doubled its employee count in 18 months (current headcount 2500), with offices across North America, Europe, and Asia-Pacific. Internal IT services supported the full employee base through a Confluence-based knowledge environment and an AI-powered assistant integrated with Slack.

## Challenge

The company's knowledge infrastructure had not scaled with its headcount. The Confluence environment contained approximately 100 spaces, roughly half actively used, with no governance model, no content architecture, no ownership framework, and no systematic connection between what employees asked and what the knowledge base contained.

Four structural gaps were compounding with each month of growth:

| Gap | What It Means |
|-----|---------------|
| **Discovery** | Content existed but could not be found. No taxonomy, no naming conventions, no information architecture. Employees defaulted to filing tickets or asking in chat rather than searching the knowledge base. |
| **Authority** | Content was found but could not be trusted. No lifecycle status, no ownership indicators, no way to distinguish a current article from an outdated page. |
| **Freshness** | Content degraded invisibly. No review dates, no staleness indicators. Articles accurate before the headcount doubled now described deprecated processes. |
| **Transfer** | Knowledge lived in people, not systems. Specialist knowledge (identity management, device management, cloud infrastructure) was concentrated in individuals. When unavailable, tickets piled up unanswered. |

These gaps formed a reinforcing cycle and directly impacted three operational areas: the AI assistant underperformed because it could only resolve what was properly documented; employees in international offices outside North American business hours had no IT support beyond what the knowledge base contained; and contractor access was managed ad hoc with no documented framework, creating compliance exposure.

## Approach

### Discovery

The assessment drew on stakeholder conversations across multiple functions (IT operations, learning and development, compliance, engineering leadership) and technical analysis of the knowledge platform configuration, including AI assistant integration mechanics and content ingestion requirements.

### Diagnostic Framework

Applying Knowledge-Centered Service (KCS) methodology revealed that the four gaps were not independent problems but a reinforcing cycle: knowledge not captured from specialists (Transfer) led to stale content (Freshness), which eroded trust (Authority), which caused employees to stop searching (Discovery), which deepened the transfer gap. Breaking the cycle at any point would produce benefits at all others.

### Methodology

All recommendations were grounded in KCS, selected because it addresses the exact operating model: a growing organization where specialist knowledge must be accessible beyond the individuals who hold it, where self-service is the primary support channel for distributed offices, and where an AI layer depends on structured content to function.

## Solution Design

The strategy was organized in two phases across 180 days, built on three principles:

| Principle | What It Means |
|-----------|---------------|
| **Governance before content** | Define architecture and ownership before creating articles. Content without structure is how the organization reached 100 ungoverned spaces in the first place. |
| **Demand-driven priorities** | Ticket data determines what gets documented first, not editorial judgment. The top repeated ticket categories become the first content sprint. |
| **Distributed ownership** | The knowledge management function builds the system; subject matter experts maintain their content within it. |

### Phase 1: Establish (Days 1-90)

**Audit and diagnose.** Complete knowledge base inventory with classification (keep, merge, archive, reassign) and permission mapping. 90-day ticket analysis to identify the top repeated categories by volume. AI assistant baseline to establish current deflection rate and content ingestion scope.

**Architecture and governance.** A tiered space architecture with defined access levels and AI ingestion scope per tier. Required metadata on every article (status, owner, content type, last reviewed, audience). A four-stage content lifecycle (Draft, In Review, Published, Archived) with strict rules: no backward transitions, no deletion, 90-day freshness triggers.

**Contractor access matrix.** Documented framework mapping space types to contractor access levels, provisioned through identity management groups and reviewed quarterly. Designed to close the compliance gap.

**First content sprint.** Top repeated ticket categories documented through a structured process: pull ticket data, capture knowledge from the subject matter expert, review, publish, tag for AI ingestion, and measure ticket volume reduction.

**Templates and review cadence.** A small set of page templates for distinct content types (how-to articles, FAQs, runbooks, SOPs, onboarding guides). Monthly article freshness reviews, quarterly space health checks, monthly AI assistant performance reviews, quarterly compliance reviews.

### Phase 2: Build (Days 91-180)

**Distributed ownership activation.** Named content owners for each specialty area, trained on the governance model, operating within a weekly rhythm. The knowledge management function provides quality checks, not central authorship.

**Runbook program.** Core operational procedures documented with specialists, covering the knowledge that currently lives in individual team members' heads. Reduces operational risk when any specialist is unavailable.

**AI assistant optimization.** Ingestion scope review, content quality audit against governance standards, query analysis to identify unanswered categories, and iterative monthly improvement feeding unresolved queries back into the content roadmap.

**Compliance controls.** Governance model positioned as compliance infrastructure: documented access matrix, no-deletion archival policy, version-controlled procedures with review dates, and offboarding documentation for content ownership reassignment.

**Cross-functional alignment.** Platform clarity between the learning management system (formal learning), the knowledge base (operational reference), and the customer-facing support platform. Working partnership with learning and development so training materials stay current as the architecture evolves.

## Deliverables

The engagement produced a single comprehensive strategic advisory report containing:

1. **Current-state assessment** structured around the four-gap diagnostic framework, with specific analysis of AI assistant performance dependencies, follow-the-sun coverage implications, and compliance exposure.

2. **180-day phased strategy** with week-by-week sequencing, role assignments, and deliverable checkpoints across two phases.

3. **Governance model** including space architecture, metadata schema, content lifecycle, naming conventions, contractor access matrix, and structural principles for scalable governance. See [condensed version](governance-model.md).

4. **Success measurement framework** with activity KPIs (content production, metadata completeness), leading KPIs (ticket deflection, AI resolution rate, content freshness), and outcome KPIs (employee self-service satisfaction, follow-the-sun coverage improvement).

5. **Strategic roadmap** for beyond the 180-day period: non-IT expansion, AI tool strategy, collaboration tool roadmap, and positioning knowledge management as a strategic organizational function.

## Key Design Decisions

**Governance before content.** The instinct when inheriting an ungoverned knowledge base is to start writing articles. Content without structure accumulates and recreates the problem. The architecture, ownership model, and lifecycle were defined before any new content was created.

**Ticket data as the content roadmap.** Content priorities were driven by demand (what employees actually ask), not editorial judgment (what seems important). This makes the first content sprint measurable and directly tied to operational workload reduction.

**AI performance is a content problem.** The AI assistant's underperformance was reframed from a tool configuration issue to a content governance issue. Poorly structured, outdated, or untagged articles directly cap AI resolution capability. Improving content quality is the AI investment.

**Distributed ownership for sustainability.** A previous attempt at centralized knowledge management by a single person had failed at this organization. The distributed model (the knowledge management function builds the system, specialists maintain their content) was designed to prevent the same failure mode.

## Methodology and Tools

- Knowledge-Centered Service (KCS)
- Information architecture and governance for a workplace wiki platform
- IT service management ticket analysis for content prioritization
- AI assistant integration analysis (content ingestion, query resolution, connector architecture)
- Compliance framework design (SOC 2 alignment)

---

*Coreso Collaborative provides knowledge governance consulting for organizations where internal knowledge must be structured, findable, and AI-ready. This case study is based on a strategic advisory engagement. Client details have been anonymized.*
