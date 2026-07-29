# Architecture

## Architecture Idea

AI Accountant is designed as a modular platform. The core owns clients,
documents, operations, tasks, roles, and audit. Heavy AI/OCR work is isolated
behind service contracts.

```text
Public website
    |
    v
Accountant workspace
    |
    v
Core API: clients, documents, operations, tasks, audit
    |
    +--> Metadata storage
    +--> Object storage for originals
    +--> OCR / Document Intelligence
    +--> LLM Router / AI Gateway
    +--> Bank Parser
    +--> 1C / EDI / banks / tax services / email
```

## Principles

- Human-in-the-loop: AI does not mutate accounting state without approval.
- Audit-first: material actions are logged.
- Tenant isolation: data is separated between organizations.
- Provider boundary: LLM, OCR, and PDF parsing are connected through contracts.
- Explainability: important suggestions include basis, confidence, and status.
- Fail closed: provider failures must not silently produce unsafe conclusions.
- Privacy by design: documents and personal data require controlled storage,
  access, retention, and logging.

## Target Components

| Component | Responsibility |
| --- | --- |
| Frontend | Public website, login, accountant workspace |
| Core API | Clients, documents, operations, reconciliation, tasks |
| Auth | Sessions, roles, tenant context, production MFA |
| Metadata DB | Structured data, states, relationships, history |
| Object Storage | Original documents and uploaded files |
| OCR Service | Scanned document and image recognition |
| PDF Parser | Text and table extraction from PDF bank statements |
| LLM Router | Providers, limits, fallback, cost modes |
| RAG | Versioned normative sources |
| Connectors | 1C, EDI, banks, tax services, email, CRM |
| Observability | Logs, metrics, incidents, AI quality |

## Pilot Profile

A practical pilot may use a hybrid setup:

- Next.js and Vercel for the public website and panel;
- isolated OCR/PDF service in a container;
- LLM through an external API provider;
- document database for metadata;
- object storage for originals in the next phase;
- real integrations added gradually through sandbox contracts.

## Production Profile

Production requires:

- durable original-document storage;
- backups and restore tests;
- MFA and expanded roles;
- sensitive-data access logs;
- retention and deletion policies;
- client and organization isolation;
- rate limits and OCR overload protection;
- observability, incident runbook, and release evidence;
- legal review for personal-data processing.

## Why Not One Big AI Chat

Accounting work requires evidence. AI Accountant is therefore designed as an
operating system around documents, operations, and decisions rather than a chat
interface alone.

Chat can be one interaction surface, but the product foundation is data, states,
tasks, approvals, sources, and audit.

