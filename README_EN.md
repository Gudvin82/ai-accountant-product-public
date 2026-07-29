# AI Accountant

**AI Accountant** is a product concept and architecture dossier for an
AI-assisted operations platform for accounting outsourcing teams.

The product idea is straightforward: give accountants and managers one
operational workspace for clients, primary documents, bank statements,
reconciliation, discrepancies, tasks, deadlines, AI suggestions, and approval
history.

AI does not replace the accountant. It recognizes, matches, suggests,
prioritizes, and explains. The final decision stays with a human specialist.

> This is a public portfolio repository. It does not contain source code,
> credentials, client data, private deployment details, or internal prompts.

## Who It Is For

- Accounting outsourcing firms.
- Heads of accounting teams.
- Accountants managing many legal entities.
- Teams that want less manual reconciliation and more operational control.
- Companies that need document, payment, and deadline visibility without
  relying on folders, messengers, and spreadsheets.

## Core Value

AI Accountant turns fragmented document and statement processing into a managed
workflow:

- documents enter one workspace;
- fields, amounts, dates, and counterparties are extracted automatically;
- bank operations are normalized and matched to documents;
- discrepancies become assigned tasks;
- AI drafts journal entries and client questions;
- accountants review, approve, or correct;
- managers see workload, delays, risks, and quality metrics.

## Product Principle

**AI suggests, the accountant confirms.**

The platform should not make final tax, accounting, or legally significant
decisions on its own. Every material result should include:

- source data;
- recognition or matching confidence;
- reasoning;
- review status;
- responsible human;
- audit trail.

## Key Documents

- [Product Description](./docs/en/product.md)
- [Features](./docs/en/features.md)
- [Architecture](./docs/en/architecture.md)
- [Use Cases](./docs/en/use-cases.md)
- [Security And Compliance](./docs/en/security.md)
- [Roadmap](./docs/en/roadmap.md)
- [Product Status](./docs/en/status.md)
- [FAQ](./docs/en/faq.md)

## Status

The pilot product contour has been designed and partially implemented in a
private working version:

- public website;
- login and work panel;
- client dashboard;
- document upload;
- OCR/PDF processing via an isolated service;
- bank data import and normalization;
- basic reconciliation;
- draft journal entries with human approval;
- task and deadline layer;
- security and architecture baseline.

Production launch requires a separate phase: durable document storage, backups,
MFA, expanded roles, legal review for personal-data compliance, and real
integrations with 1C, EDI, banks, tax services, and email.

## What This Repository Does Not Include

- production source code;
- real client documents;
- API keys or tokens;
- passwords or access data;
- internal infrastructure addresses;
- private business agreements.

## Methodology

The dossier is organized as product engineering work:

- Vibe Coding Protocols: intent, control, proof, and gates;
- strong engineering practice: contracts, boundaries, observability;
- GitHub Spec Kit style: specifications, plans, tasks, acceptance criteria;
- honest separation of `implemented`, `designed`, and `roadmap`.

## Author

Created by Anatoliy Malyshev as part of an AI product, automation, and product
architecture portfolio.

