# AI Risk Model

## Approach

AI Accountant uses AI as workflow support, not as an autonomous accountant. The
goal of the risk model is to make AI outputs verifiable, bounded, and
governable.

## Risk Table

| Risk | Example | Mitigation |
| --- | --- | --- |
| Hallucination | AI cites a non-existent rule | sources, effective dates, refusal behavior |
| Wrong classification | expense assigned to the wrong category | human approval, confidence, correction history |
| OCR error | amount or tax ID extracted incorrectly | field confidence, disputed-field highlighting |
| Outdated rule | answer uses an old regulation | versioned RAG and source date |
| Data exposure | document sent to an unsuitable provider | provider allowlist, tenant isolation, secrets outside code |
| Silent provider failure | fallback shown as a real answer | fail closed, explicit error status |
| Uncontrolled automation | journal entry reaches accounting without review | approval gate before mutation or export |
| Lost evidence | unclear why a decision was made | audit trail and preserved basis |
| Duplicates | repeated webhook/import creates a second object | idempotency key and replay log |
| Client mix-up | document assigned to the wrong tenant | tenant context and ownership checks |

## AI Output Requirements

A material AI output should include:

- suggestion;
- source data;
- confidence;
- limitations;
- sources for normative answers;
- human review status;
- rejection path.

## Kill Switch

The production architecture needs a fast way to disable:

- LLM answers;
- automatic drafts;
- export;
- a specific provider;
- an integration channel.

This allows the team to continue manual work even when the AI layer has issues.

