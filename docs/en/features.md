# Features

## Feature Status

| Capability | Status | Comment |
| --- | --- | --- |
| Public website | Pilot | published as the external product entry |
| Work panel | Pilot | private working version |
| Clients and search | Pilot | basic operations contour |
| Document upload | Pilot | UI and processing contour |
| OCR/PDF extraction | Pilot contour | isolated service contract |
| CSV statements | Pilot | deterministic normalization |
| Basic reconciliation | Pilot | amount, date, counterparty |
| Draft journal entries | Pilot | approval required |
| Tasks and deadlines | Pilot | basic control layer |
| Object storage | Roadmap | required before real-data production |
| MFA and expanded roles | Roadmap | production gate |
| 1C/EDI/banks/tax/email | Roadmap | sandbox-first integration path |
| Normative RAG | Designed | enable only after source evaluation |

## Client Workspace

- Unified client and organization registry.
- Client card with documents, operations, tasks, and history.
- Search, filters, processing states, and responsible users.
- Period control: accepted items, missing documents, and items requiring review.

## Documents

- Upload invoices, acts, transfer documents, receipts, contracts, and scans.
- Extract date, amount, counterparty, tax IDs, document type, and other fields.
- Field-level confidence.
- Manual correction while preserving the original extraction.
- Processing status for every document.

## Bank Statements

- Import CSV and PDF statements.
- Normalize operations.
- Categorize payments.
- Link payments to source documents.
- Prepare operations for reconciliation and export.

## Reconciliation

- Match by amount, date, counterparty, and payment purpose.
- Detect discrepancies.
- Target discrepancy classes:
  - payment without document;
  - document without payment;
  - amount mismatch;
  - wrong legal entity;
  - duplicate;
  - split or combined payment;
  - suspicious payment purpose.

## Journal Entries And Approval

- AI drafts journal entries.
- The accountant sees basis and context.
- The accountant can approve, correct, or reject.
- The decision is stored in history.
- Unapproved suggestions must not reach the accounting system of record.

## Tasks And Deadlines

- Automatically create tasks from discrepancies.
- Assign responsible users.
- Track deadlines and overdue items.
- Document review queue.
- Manager view of problematic clients.

## AI Layer

- Document recognition and explanation.
- Matching suggestions.
- Draft client questions.
- Draft journal entries.
- Normative help only with sources, effective dates, and review status.

## Integrations

Target integrations:

- 1C;
- EDI;
- banks;
- tax services;
- email;
- CRM;
- object storage;
- LLM and OCR providers through isolated contracts.

## Analytics

- Accepted and rejected AI suggestions.
- Time per processed document.
- OCR fields accepted without correction.
- Number and classes of discrepancies.
- SLA and overdue tasks.
- Clients per accountant.
- Processing cost per document and per client.
