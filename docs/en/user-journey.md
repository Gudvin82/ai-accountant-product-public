# User Journey

## Scenario: Incoming Invoice And Bank Payment

This scenario shows the product as one accountant workflow rather than a set of
modules.

## 1. Document Enters The Workspace

The client sends an invoice or transfer document. The accountant uploads it to
the client card.

The system creates a document record and stores:

- client;
- upload timestamp;
- file type;
- actor;
- processing status.

## 2. OCR Extracts Fields

The OCR/PDF service extracts:

- counterparty;
- tax IDs;
- date;
- amount;
- VAT;
- document number;
- document type.

Low-confidence fields are highlighted for manual review.

## 3. The System Searches For A Related Payment

The bank parser normalizes the statement. The reconciliation layer searches by:

- amount;
- date;
- counterparty;
- payment purpose;
- client's legal entity.

## 4. A Discrepancy Appears

For example, a payment is found but the amount does not match the document, or
the payment purpose references another contract.

The system creates a task and shows the accountant:

- where the discrepancy is;
- which data was used;
- how confident the match is;
- what can be done next.

## 5. AI Prepares A Draft

AI suggests:

- possible reason for the discrepancy;
- draft client question;
- draft journal entry if enough data exists;
- warning if confidence is low.

The AI draft is not a final decision.

## 6. The Accountant Decides

The accountant can:

- approve the match;
- correct extracted fields;
- reject the AI suggestion;
- send a client question;
- assign a task to a colleague;
- postpone until the missing document arrives.

## 7. The Decision Is Recorded

The audit trail records:

- source document;
- extracted fields;
- related payment;
- AI suggestion;
- accountant action;
- correction or rejection reason;
- timestamp and responsible user.

## 8. The Manager Sees The Outcome

The management layer shows:

- how many documents were processed;
- where discrepancies remain;
- which clients delay the period;
- which tasks are overdue;
- how many AI suggestions were accepted or rejected.

