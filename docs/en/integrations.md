# Integration Map

## Position

AI Accountant should not become another isolated accounting system. The goal is
to act as an operational layer above the accountant's existing tools.

## Integration Map

| Integration | Purpose | Public status |
| --- | --- | --- |
| File upload | Manual import of documents and statements | Pilot |
| CSV statements | Fast import of bank operations | Pilot |
| PDF statements | Extract operations from PDF files | Pilot contour |
| OCR service | Recognize scans and images | Pilot contour |
| LLM provider | Drafts, explanations, classification | Designed |
| Object storage | Original documents | Roadmap |
| 1C | Export approved data | Roadmap |
| EDI | Receive primary documents | Roadmap |
| Banks | Automatic statement retrieval | Roadmap |
| Tax services | Verification and normative scenarios | Roadmap |
| Email | Incoming documents and client responses | Roadmap |
| CRM | Clients, states, communications | Roadmap |
| Excel | Import/export during transition | Roadmap |

## Integration Principles

- Idempotency: repeated delivery must not create duplicates.
- Audit trail: imports, exports, and errors are recorded.
- Sandbox-first: fixtures and replay before real credentials.
- Human approval: disputed actions are not executed automatically.
- Least privilege: access only to required data.
- Provider isolation: credentials and channels are not shared between projects.

## 1C

Recommended path:

1. Select one configuration and version.
2. Build one-way export for approved data.
3. Add error reports and replay.
4. Preserve links between exported objects, source documents, and decisions.
5. Move to bidirectional synchronization only after export evidence is stable.

