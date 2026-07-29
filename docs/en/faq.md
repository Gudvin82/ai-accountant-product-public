# FAQ

## Is this an open-source product?

No. This is a public product dossier and showcase. The working source code is
private.

## Why no code?

Because the product touches accounting workflows, integrations, secrets,
infrastructure, and potentially sensitive data. The public repository shows
product depth without exposing implementation details.

## Does AI do accounting by itself?

No. AI prepares suggestions and explanations. The accountant approves, corrects,
or rejects them.

## Can this replace 1C?

No. The product is designed as an operational layer above existing accounting
systems, not as a replacement for 1C.

## Who is it primarily for?

Accounting outsourcing teams that manage many clients and want to control
documents, statements, discrepancies, tasks, and deadlines in one place.

## What is the most important architecture idea?

Separation of responsibility:

- the core product stores states, relationships, tasks, and audit;
- OCR and LLM work through isolated contracts;
- humans confirm outcomes;
- important actions are logged.

## What is needed before production launch?

Durable document storage, backups, MFA, roles, personal-data legal review,
retention policy, observability, and real integrations.

