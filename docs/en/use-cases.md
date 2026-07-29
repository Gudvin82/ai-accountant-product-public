# Use Cases

## 1. Closing A Period For A Client

The accountant opens a client and sees the period state:

- documents uploaded;
- bank operations imported;
- payments already matched;
- open discrepancies;
- overdue tasks;
- decisions waiting for approval.

Outcome: less manual searching and more control before period close.

## 2. Primary Documents From Multiple Sources

Documents arrive through upload, email, EDI, or a client channel. The system
extracts fields, groups documents by client, highlights low confidence, and asks
the accountant to verify questionable fields.

Outcome: source documents enter processing faster and are less likely to get
lost.

## 3. Matching A Payment To A Document

The system finds a bank operation and tries to link it to a document by amount,
date, counterparty, and payment purpose.

If the match is reliable, the accountant approves it. If there is a problem, a
task is created: request a document, check a contract, clarify payment purpose,
or contact the client.

## 4. Draft Journal Entry

AI suggests a journal entry based on a document, bank operation, tax regime, and
client context.

The accountant sees:

- what was suggested;
- why the system suggested it;
- which data was used;
- how confident the system is;
- what requires manual review.

After review, the accountant approves or corrects the result.

## 5. Client Request

If a payment does not match a document or the document is missing, the system
drafts a client question.

The accountant edits and approves the message. The client response returns to
the task card.

## 6. Manager Workflow

The manager sees:

- accountant workload;
- problematic clients;
- discrepancy count;
- overdue items;
- accepted and rejected AI suggestions;
- recognition and reconciliation quality.

Outcome: management is based on evidence, not manual reports.

## 7. Preparing Export To 1C

Approved documents, operations, and journal entries are collected into an export
package.

Target principle: start with one-way, idempotent, auditable export. Bidirectional
synchronization should come only after export evidence is stable.

