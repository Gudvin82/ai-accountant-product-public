# Product Status

## Purpose

This document clearly separates:

- what exists in the working contour;
- what has been designed;
- what belongs to the roadmap;
- what should not be treated as production-ready yet.

## Public Repository

Status: ready as a product showcase.

This repository contains product description, architecture, use cases, security,
and roadmap. It does not contain source code or secrets.

## Pilot Contour

Status: partially implemented in a private working version.

| Layer | Status | Comment |
| --- | --- | --- |
| Public website | Pilot | external entry and pilot request |
| Login | Pilot | route to the private work contour |
| Client dashboard | Pilot | search, filters, basic states |
| Document upload | Pilot | UI and processing through a service contract |
| OCR/PDF contour | Pilot contour | isolated provider boundary |
| Bank data import | Pilot | CSV and PDF direction |
| Basic reconciliation | Pilot | first matches and discrepancies |
| Draft journal entries | Pilot | human approval required |
| Tasks and calendar | Pilot | basic deadline control |
| Production storage | Roadmap | required before real data |
| 1C/EDI/banks/tax/email | Roadmap | real credentials and contracts separately |

## Designed

- Target modular architecture.
- AI/OCR provider boundaries.
- Human approval boundary.
- Future connector contracts.
- Production security baseline.
- Path to 1C export.
- Phase-based roadmap.

## Roadmap / Not Fully Ready Yet

- Long-term original-document storage.
- Off-host backups.
- MFA.
- Expanded roles and invitations.
- Retention and deletion policies.
- Full legal review for personal-data compliance.
- Real integrations with 1C, EDI, banks, tax services, and email.
- Normative RAG with verified sources.
- OCR scale-out.
- Production-grade management analytics.

## Honest Assessment

| Area | Assessment |
| --- | --- |
| Product concept | strong |
| Pilot UX | strong |
| Architecture direction | formed |
| Production backend | next phase required |
| Compliance readiness | specialist review required |
| Integrations | roadmap |

## Why This Status Is Stronger

The repository does not pretend to be a complete open-source product. It shows
product maturity: a clear problem, target audience, architecture, constraints,
risk control, and development plan.

For a portfolio, this is often stronger than a code repository without product
context.
