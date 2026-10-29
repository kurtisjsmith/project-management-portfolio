# Master Project Management Standard

**Version:** 1.0
**Approved:** October 27, 2026
**Status:** Approved
**Document Owner:** Project Owner / Project Manager
**Applicability:** All projects formally adopting this standard

---

## 1. Purpose

Establish a consistent, professional, and reusable system for managing projects from initiation through closure.

The standard supports project planning, implementation, research, documentation, verification, decision-making, and portfolio oversight.

Project management must facilitate measurable progress and completion rather than become an ongoing activity without defined outcomes.

## 2. Governance Principles

1. **Accountability:** The Project Owner retains final decision authority.
2. **Single Source of Truth:** Each authoritative record has one designated location.
3. **Stable Baselines:** Preserve approved project frameworks unless changes are justified and authorized.
4. **Evidence-Based Progress:** Distinguish planned, implemented, verified, and formally closed work.
5. **Controlled Scope:** New findings do not automatically expand approved requirements.
6. **Traceability:** Preserve significant decisions, changes, verification evidence, and historical context.
7. **Proportionality:** Documentation and controls should match the project's size, complexity, and risk.
8. **Continuous Improvement:** Apply lessons learned without unnecessarily reopening completed work.

## 3. Management Roles and Authority

### 3.1 Project Owner and Project Manager

The individual responsible for the project holds both roles unless responsibility is explicitly assigned otherwise.

Responsibilities include:

- Establishing project objectives and priorities.
- Approving scope, requirements, and acceptance criteria.
- Authorizing project changes.
- Evaluating risks and tradeoffs.
- Monitoring milestones and progress.
- Accepting deliverables.
- Approving formal phase and project closure.

### 3.2 AI Assistant

The **AI Assistant** supports the Project Owner and Project Manager in project-management activities.

Responsibilities include:

- Supporting planning and documentation.
- Reviewing progress against agreed milestones.
- Identifying risks, blockers, inconsistencies, and scope drift.
- Recommending changes with supporting reasoning.
- Preparing progress reports and handoffs.
- Distinguishing approved decisions from proposals and assumptions.

The AI Assistant must not independently authorize changes to approved project requirements or modify project assets without appropriate authorization.

The role is provider-independent and may be performed by different AI systems, including locally hosted or personally developed models.

**Authority Decision:** PM-01-D01.

## 4. Project Initiation Requirements

Before beginning implementation, each new project should establish:

1. **Purpose:** Why the project exists.
2. **Objectives:** What outcomes the project intends to achieve.
3. **Scope:** What is included and excluded.
4. **Deliverables:** What the project will produce.
5. **Constraints:** Relevant time, resource, technical, or operational limitations.
6. **Initial Risks and Dependencies:** Known uncertainties and prerequisites.
7. **Initial Roadmap:** Major phases or milestones.
8. **Authorization:** Approval to proceed with the defined initial scope.

Project initiation should be proportional to complexity. Small projects may record this information directly in `PROJECT_MANAGEMENT.md`.

Initiation approval does not automatically authorize every future milestone or implementation change.

## 5. Documentation Authority

### 5.1 Master Repository

The master Project Management repository maintains:

- Shared governance standards.
- Reusable documentation templates.
- Common terminology and procedures.
- Portfolio-level status references.
- Cross-project lessons and improvement proposals.

### 5.2 Individual Project Repositories

Each project repository is authoritative for its own:

- Objectives and requirements.
- Roadmap and milestones.
- Project status.
- Architecture and implementation plans.
- Decisions and approval records.
- Verification and closure evidence.

### 5.3 AI-Assisted Conversations

Conversations with an AI Assistant support collaborative reasoning, reviews, and handoffs but are not the durable system of record.

Approved decisions should be recorded in the relevant repository.

**Authority Decision:** PM-01-D02.

## 6. Minimum Project Documentation

Each managed project normally maintains three core documents:

| Document                | Responsibility                                                                    |
| ----------------------- | --------------------------------------------------------------------------------- |
| `README.md`             | Introduction, usage, setup, and documentation navigation                          |
| `PROJECT_MANAGEMENT.md` | Project charter, roadmap, milestone register, progress, and governance references |
| `DECISION_LOG.md`       | Significant decisions, rationale, approval dates, and supersession history        |

Additional documentation may include:

- Design specifications.
- Implementation plans.
- Architecture records.
- Risk and issue registers.
- Audits and verification reports.
- Research and experiment records.
- Handoffs and closure reports.

Additional documents are created only when justified by the project's requirements.

Existing projects adopt this standard incrementally without unnecessary restructuring, duplication, or loss of historical evidence.

**Authority Decision:** PM-01-D03.

## 7. Standard Status Vocabulary

| Status    | Definition                                                                                     |
| --------- | ---------------------------------------------------------------------------------------------- |
| Planned   | Recognized and approved for future consideration or scheduling; implementation has not started |
| Active    | Authorized work is underway                                                                    |
| Blocked   | A documented obstacle prevents progress                                                        |
| Deferred  | Intentionally postponed                                                                        |
| Completed | Agreed acceptance criteria have been satisfied and verified                                    |
| Closed    | Completion has been formally reviewed, recorded, and approved                                  |

These labels apply consistently to projects, phases, milestones, and workstreams where appropriate.

A completed milestone is not automatically closed.

## 8. Project and Milestone Lifecycle

The standard lifecycle is:

**Define → Execute → Verify → Close**

Every milestone identifies:

- Objective and deliverable.
- Scope and exclusions.
- Acceptance criteria.
- Verification method.
- Current status.
- Implementation and verification evidence.
- Closure decision and date.

Acceptance criteria must be defined before implementation or investigation begins.

For research projects, acceptance criteria may concern methodology, reproducibility, documented findings, or completion of a defined investigation rather than a predetermined scientific conclusion.

### 8.1 Milestone Completion

A milestone becomes **Completed** when its agreed acceptance criteria have been satisfied and verified.

A milestone becomes **Closed** after formal approval and documentation of its closure.

### 8.2 Milestone Reopening

A closed milestone may be reopened only when a verified critical defect or unmet agreed acceptance criterion justifies doing so.

The reason must be documented, and the Project Owner must approve reopening.

**Authority Decision:** PM-01-D04.

## 9. Phase Completion Requirements

Each phase must have defined completion requirements before execution begins.

A phase may be marked **Completed** when all applicable requirements have been satisfied:

1. **Defined Scope:** Approved purpose, deliverables, boundaries, and exclusions.
2. **Acceptance Criteria:** All agreed criteria have been satisfied or explicitly revised through change control.
3. **Implementation Evidence:** Required deliverables have been produced with supporting evidence.
4. **Verification:** Applicable tests, reviews, inspections, or research validation activities have passed.
5. **Defect Assessment:** No unresolved blocking defects remain within approved scope.
6. **Outstanding Work Classification:** Remaining findings are recorded as blockers, in-scope requirements, deferred enhancements, or separate workstreams.
7. **Documentation Reconciliation:** Authoritative records accurately reflect completed work, evidence, decisions, and limitations.
8. **Next-Phase Readiness:** The next milestone or phase is identified, including dependencies and prerequisites.

### 9.1 Phase Closure Requirements

A phase becomes **Closed** only after:

- Its completion requirements have been verified.
- The Project Owner has approved closure.
- A closure record identifies the phase, date, verification evidence, known limitations, and transferred or deferred work.
- The authoritative project-management document records the closure decision.

Closure of a phase does not mean the entire project is complete.

### 9.2 Scope Protection and Reopening

Additional improvements or future requirements do not automatically prevent phase completion or reopen a closed phase.

A verified critical defect or unmet agreed acceptance criterion may justify reopening with documented reasoning and Project Owner approval.

Otherwise, new findings are classified and assigned to an appropriate future milestone or workstream.

**Governing Principle:** Phase completion is determined by agreed criteria and verification evidence, not by the absence of possible future improvements.

## 10. Change Control

Changes are evaluated proportionally.

| Classification         | Required Handling                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------- |
| Routine Implementation | Proceed within existing authorization                                                   |
| Minor Adjustment       | Record reason and relevant impact                                                       |
| Material Change        | Explicit Project Owner approval                                                         |
| Critical Defect        | Investigate promptly; corrective implementation requires authorization and verification |

Material changes include alterations to approved scope, acceptance criteria, architecture, priorities, or milestones.

New findings must be classified as:

1. Blocking defect.
2. Existing in-scope requirement.
3. Deferred enhancement.
4. Separate workstream.

The AI Assistant must identify when its recommendations would expand approved scope.

**Authority Decision:** PM-01-D05.

## 11. Review and Audit Control

Every review or audit must establish:

- A defined purpose.
- A bounded scope.
- Identified evidence requirements.
- A completion condition.
- An expected decision or deliverable.

Once the agreed completion condition is satisfied, the review ends.

Previously completed inspections must not be repeated without a specific justification, such as changed requirements, new evidence, or a verified defect.

Reviews should produce actionable conclusions rather than generating additional investigations indefinitely.

## 12. Verification and Evidence

Progress claims must distinguish:

- Proposed behavior.
- Approved requirements.
- Implemented behavior.
- Verified behavior.
- Formally accepted deliverables.

Verification evidence may include:

- Automated test results.
- Manual testing records.
- Experimental findings.
- Repository commits.
- Inspections and reviews.
- Approved acceptance records.

Evidence must be relevant to the specific claim.

A passing test suite supports the behaviors it covers; it does not certify every aspect of a system.

## 13. Progress Monitoring and Reporting

Each active project should maintain a concise progress record containing:

- Current phase and milestone.
- Current status.
- Latest verified accomplishment.
- Active blockers, risks, or dependencies.
- Next authorized action.
- Date of last verification.

Progress records should be updated at milestone boundaries, significant decisions, or meaningful changes in project status.

Reporting must distinguish verified progress from reported or assumed progress.

Avoid duplicating complete technical records in portfolio summaries or management reports.

## 14. Collaboration and Implementation

The standard collaborative workflow is:

**Inspect → Discuss → Propose → Approve → Implement → Verify → Commit**

The Project Owner retains implementation and change authority.

The AI Assistant must:

- Preserve existing project files and records.
- Avoid destructive operations without authorization.
- Present reviewable changes.
- Respect previously approved requirements.
- Support incremental implementation and verification.
- Avoid unnecessary changes outside the authorized scope.

Existing project-specific workflows remain applicable unless explicitly revised.

## 15. AI Assistant Accountability

The AI Assistant is responsible for supporting disciplined project execution.

It must:

1. **Respect Established Decisions:** Consult available project decisions and authoritative documentation before recommending changes.
2. **Prevent Review Loops:** Avoid repeating completed investigations without new justification.
3. **Identify Scope Drift:** Clearly state when a recommendation introduces work beyond an approved milestone.
4. **Maintain Evidence Integrity:** Distinguish verified facts from assumptions, estimates, and reported information.
5. **Respect Closure:** Do not reopen completed phases or milestones without a documented justification and Project Owner approval.
6. **Preserve Continuity:** Reference existing progress and decisions rather than repeatedly restarting project analysis.
7. **Communicate Limitations:** Identify unavailable evidence, uncertain conclusions, and actions not actually performed.
8. **Support Project Ownership:** Explain reasoning and tradeoffs so the Project Owner retains understanding and control.

AI assistance must improve project clarity and productivity rather than create unnecessary administrative activity.

## 16. Risk, Issue, and Decision Management

Risks concern possible future events; issues concern conditions already present.

Significant risks and issues should identify:

- Description.
- Potential or observed impact.
- Responsible owner.
- Current status.
- Next action or mitigation.

Significant decisions should record:

- Decision identifier.
- Date.
- Context and rationale.
- Approved outcome.
- Authorizing individual.
- Superseded decisions, where applicable.

Do not duplicate complete decision records across multiple authoritative documents.

## 17. Handoffs and Continuity

Handoffs are an established operational practice for preserving project continuity across conversations, devices, work sessions, and project transitions.

The AI Assistant should proactively recommend a handoff when:

- A conversation becomes lengthy or risks losing important context.
- Work transitions between devices, projects, or conversations.
- A significant architectural or management decision is made.
- A milestone or phase is completed.
- A new phase or substantial workstream begins.

Handoffs should summarize:

- Verified current state.
- Completed work.
- Active phase and milestone.
- Significant decisions and applicable constraints.
- Outstanding issues, risks, and dependencies.
- Next authorized action.

Handoffs support continuity but do not replace authoritative project documentation.

Significant decisions, milestone completion, and formal closure must also be recorded in their designated project records.

Not every handoff requires a permanent repository file. Preserve handoffs when their continuing operational or historical value justifies retention.

## 18. Portfolio Management

The master repository may maintain a portfolio register referencing individual projects.

The register should identify:

- Project name and authoritative repository.
- Current phase and milestone.
- Status and priorities.
- Significant dependencies or blockers.
- Latest verified progress.
- Next authorized action.

Portfolio records should reference project documentation instead of reproducing detailed technical information.

## 19. Documentation Maintenance

Preserve stable framework language wherever practical.

Update current status, milestones, evidence references, and decisions as work progresses.

Avoid restructuring established documents solely for cosmetic uniformity.

Documentation reviews must have defined objectives and completion conditions.

Historical records should be preserved and marked superseded when appropriate rather than silently rewritten.

## 20. Project Closure and Lessons Learned

Formal project closure should record:

- Accepted deliverables.
- Verification evidence.
- Known limitations.
- Deferred or transferred work.
- Relevant lessons learned.
- Approval and closure date.

Lessons learned may inform future projects without automatically reopening completed work.

## 21. Standard Adoption and Revision

Projects adopt this standard through explicit approval.

The standard is maintained under version control.

Material amendments require documented reasons, impact assessment, and Project Owner approval.

Minor editorial corrections may be made through the normal authorized review process.

Revisions to the master standard do not automatically rewrite existing project decisions, requirements, or acceptance criteria.

---

**Foundational Rule:** Project management must provide direction, accountability, traceability, and verifiable completion—not perpetual review or unnecessary activity.