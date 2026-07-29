# Security And Compliance

## Position

AI Accountant handles accounting documents, personal data, financial operations,
and potentially sensitive commercial information. Security is therefore part of
the product, not an afterthought.

## Baseline Requirements

- Client and organization isolation.
- Roles and access control.
- MFA for admins and owners.
- Secrets outside source code.
- HTTPS and secure cookie sessions.
- Audit log for material actions.
- Sensitive-data read log.
- Upload validation.
- AI/OCR provider allowlist.
- Backups and restore testing.
- Incident runbook.

## Data Classes

- Public product materials.
- Organization configuration.
- Client accounting data.
- Personal data.
- Primary documents.
- AI prompts and responses with sensitive context.
- Secrets and provider credentials.

## Russian Personal-Data Compliance

For real-data operation in Russia, a separate legal and security review is
required:

- define personal-data categories;
- define processing purposes;
- configure storage and deletion;
- formalize access;
- review providers and cross-border aspects;
- keep action logs;
- approve document retention policy;
- prepare incident response.

This repository is not a legal opinion. It records architectural requirements
that must be reviewed by legal and information-security specialists before
production use.

## AI Safety

The AI layer should:

- avoid final decisions without human approval;
- avoid unknown sources for normative answers;
- show source effective dates;
- refuse unsupported conclusions;
- preserve decision evidence;
- separate drafts from confirmed results.

## Production Gate

Before production launch, the following must be closed:

- MFA;
- roles and tenant isolation;
- object storage;
- off-host backups;
- restore tests;
- retention and deletion policy;
- access audit;
- provider review;
- release decision with evidence.

