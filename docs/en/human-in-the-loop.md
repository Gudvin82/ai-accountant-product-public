# Human-in-the-loop

## Core Principle

AI Accountant is built around one rule:

> AI suggests, the accountant confirms.

This is not a decorative phrase. It is the responsibility boundary of the
product. In accounting, mistakes may have financial and legal consequences, so
AI should support the professional rather than replace the decision.

## Workflow

```text
Document or operation
    |
    v
AI extracts, matches, or suggests
    |
    v
The system shows basis, confidence, and risk
    |
    v
The accountant approves, corrects, or rejects
    |
    v
The decision is stored in the audit trail
    |
    v
Future similar cases receive better context
```

## Where Human Review Is Required

- journal entry approval;
- correction of extracted fields;
- discrepancy resolution;
- sending a client question;
- export to the accounting system of record;
- use of normative answers;
- any low-confidence or disputed case.

## What The Accountant Should See

For every material suggestion:

- source document or operation;
- extracted fields;
- confidence;
- reason for the suggestion;
- related documents and payments;
- rules or sources;
- warnings;
- approve, correct, and reject actions.

## What Is Recorded

- who made the decision;
- what was suggested;
- what was approved or changed;
- timestamp;
- data source;
- rule or AI-provider version where applicable;
- rejection or correction reason.

## Why This Matters

Human-in-the-loop makes the product suitable for a regulated domain:

- professional responsibility remains clear;
- AI-error risk is reduced;
- evidence is preserved;
- managers can monitor decision quality;
- the system can improve from real feedback.

