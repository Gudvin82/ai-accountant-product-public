# Roadmap

This roadmap describes product direction, not a public delivery promise.

## Run 0: Public Dossier And Governance

Goal: show product depth and make boundaries visible.

Status: completed in this public repository.

- Product description.
- Feature map.
- Architecture.
- Use cases.
- Security.
- Status.
- Roadmap.
- RU/EN documentation.

## Run 1: Real-Data Pilot Foundation

Priority: P0.

- Persistent database.
- Object storage for originals.
- Roles, invitations, MFA.
- Audit trail.
- Backups.
- Restore tests.
- Retention policy.

Exit: one pilot client can safely store and process real documents with a clear
audit trail.

## Run 2: Measurable Reconciliation

Priority: P0.

- OCR with field coordinates and confidence.
- PDF bank statement parsing.
- Discrepancy classes.
- Review queue.
- Approve, correct, reject.
- Quality metrics.

Exit: the accounting team can compare manual work and AI-assisted work by time,
errors, and accepted suggestions.

## Run 3: Team Operations And Client Requests

Priority: P1.

- Draft client questions.
- Approval before sending.
- Response status.
- Reminders.
- Accountant workload.
- SLA and overdue items.
- Manager screen.

Exit: the manager controls the full cycle without manually reconstructing status
from messengers and spreadsheets.

## Run 4: 1C And Integrations

Priority: P1.

- Select the first supported 1C configuration.
- One-way export.
- Idempotency.
- Error report.
- Replay.
- Careful bidirectional sync only after evidence is stable.

Exit: approved data reaches 1C without manual re-entry while preserving a link
to the source decision.

## Run 5: Normative AI And RAG

Priority: P1/P2.

- Versioned sources.
- Effective dates.
- Refusal of unsupported conclusions.
- Answer evaluation.
- Deterministic risk rules before LLM explanations.

Exit: the AI assistant does not answer without sources and does not replace
professional review.

## Run 6: Scale And Commercial Control

Priority: P2.

- EDI/email/bank/tax/CRM connectors.
- Plans and limits.
- Unit economics.
- OCR capacity.
- Observability.
- Security drills.
- Client and management reports.

Exit: quality, cost, risks, and the commercial model are measurable.

