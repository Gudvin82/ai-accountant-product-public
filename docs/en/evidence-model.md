# Evidence Model

## Why Evidence Matters

In accounting, an "AI answer" is not enough. The team needs to understand why
the system suggested an action, which data it used, and who confirmed it.

The evidence model describes what a verifiable suggestion consists of.

## Evidence Bundle

Every material AI suggestion should include:

| Element | Purpose |
| --- | --- |
| Source document | original file or document |
| Extracted fields | tax IDs, amounts, dates, counterparty |
| Confidence | field or matching confidence |
| Matching context | related payment, document, or operation |
| Rule or source | rule, normative source, or logic |
| AI draft | suggested action or explanation |
| Human decision | approved, corrected, or rejected |
| Audit event | who did what and when |
| Version metadata | rule, model, or service version where applicable |

## Example

```text
AI suggestion:
  Suggest journal entry Dr 41 - Cr 60

Evidence:
  - Transfer document N184 dated 2026-07-15
  - Counterparty: Supplier LLC
  - Amount: 124,800.00 RUB
  - Related payment: 124,800.00 RUB
  - Confidence: 96%
  - Limitation: contract review required
  - Decision: approved by accountant
  - Audit event: user, timestamp, action
```

## What Is Not Evidence

- plain AI text;
- conclusion without a source;
- conclusion without confidence;
- conclusion without review status;
- suggestion that cannot be linked to a document or operation.

## Value

The evidence model helps:

- explain decisions;
- review errors;
- learn from corrections;
- prepare export to 1C;
- audit quality;
- reduce blind trust in AI.

