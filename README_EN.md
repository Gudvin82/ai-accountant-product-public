# AI Accountant

[![Docs](https://img.shields.io/badge/docs-RU%20%2F%20EN-blue)](./README.md)
[![Status](https://img.shields.io/badge/status-public%20product%20dossier-1f6f50)](./docs/en/status.md)
[![Source](https://img.shields.io/badge/source-private-lightgrey)](./README.md)
[![License](https://img.shields.io/badge/license-CC%20BY%204.0-green)](./LICENSE)

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
- [Human-in-the-loop](./docs/en/human-in-the-loop.md)
- [Product Limitations](./docs/en/limitations.md)
- [AI Risk Model](./docs/en/ai-risk-model.md)
- [Integration Map](./docs/en/integrations.md)
- [Pilot Metrics](./docs/en/metrics.md)
- [Security And Compliance](./docs/en/security.md)
- [Roadmap](./docs/en/roadmap.md)
- [Product Status](./docs/en/status.md)
- [FAQ](./docs/en/faq.md)
- [Changelog](./CHANGELOG.md)

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

## Product Maturity

| Layer | Status |
| --- | --- |
| Product concept | defined |
| Private pilot contour | partially implemented |
| Public documentation | published |
| Production-ready platform | roadmap |
| Source code | private |

## What This Repository Does Not Include

- production source code;
- real client documents;
- API keys or tokens;
- passwords or access data;
- internal infrastructure addresses;
- private business agreements.

## For Partners

This repository is open for pilot discussions, partnerships, and architecture
review around AI-assisted accounting operations.

- Telegram: [@a_malishev](https://t.me/a_malishev)
- GitHub: [Gudvin82](https://github.com/Gudvin82)

## Methodology

The dossier is organized as product engineering work:

- [Vibe Coding Protocols](https://github.com/Gudvin82/vibe-coding-protocols):
  intent, control, proof, and gates;
- strong engineering practice: contracts, boundaries, observability;
- GitHub Spec Kit style: specifications, plans, tasks, acceptance criteria;
- honest separation of `implemented`, `designed`, and `roadmap`.

## Author

Created by Anatoliy Malyshev as part of an AI product, automation, and product
architecture portfolio.
