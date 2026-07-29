# AI Accountant / AI-Бухгалтер

[![Docs](https://img.shields.io/badge/docs-bilingual-blue)](./README.md)
[![Status](https://img.shields.io/badge/status-public%20product%20dossier-1f6f50)](./docs/en/status.md)
[![Source](https://img.shields.io/badge/source-private-lightgrey)](./README.md)
[![License](https://img.shields.io/badge/license-CC%20BY%204.0-green)](./LICENSE)

**AI Accountant** is a product concept and implementation blueprint for an
AI-assisted operating layer for accounting outsourcing teams.

**AI-Бухгалтер** — продуктовая концепция и архитектурное досье платформы,
которая помогает бухгалтерскому аутсорсингу обрабатывать первичные документы,
банковские выписки, расхождения, задачи и клиентские запросы в одном рабочем
контуре.

> Public portfolio repository. Production source code, credentials, private
> deployment details, client data, and internal prompts are intentionally not
> included.
>
> Публичный портфолио-репозиторий. Продакшен-код, ключи, приватные детали
> инфраструктуры, клиентские данные и внутренние промпты намеренно не включены.

## Language / Язык

- [Русская версия](./README_RU.md)
- [English version](./README_EN.md)

## What This Repository Shows

- Product vision for an AI accounting operations platform.
- Target feature map and user workflows.
- Human-in-the-loop accounting approval model.
- AI risk model and explicit product limitations.
- Integration map for 1C, EDI, banks, email, tax services, and CRM.
- Business metrics for pilot validation.
- Public architecture without sensitive implementation details.
- Security and compliance principles for Russian accounting data.
- Roadmap from pilot to production-grade platform.
- Current status separated from planned capabilities.

## Что Здесь Есть

- Описание продукта для бухгалтерского аутсорсинга.
- Карта возможностей и рабочих сценариев.
- Модель, где AI предлагает, а бухгалтер подтверждает.
- Модель рисков AI и явные ограничения продукта.
- Карта интеграций с 1С, ЭДО, банками, email, ФНС и CRM.
- Бизнес-метрики для проверки пилота.
- Публичная архитектура без кода и секретов.
- Контур безопасности, хранения данных и 152-ФЗ.
- Roadmap развития от пилота до промышленной платформы.
- Честное разделение: что уже есть, что спроектировано, что в планах.

## Repository Structure

```text
docs/
  en/   English product dossier
  ru/   Русское продуктовое досье
```

## Public Status

This repository is a **showcase and product dossier**, not an open-source
release of the production system.

The working product prototype exists separately. This public repository is meant
to explain the idea, product depth, operating model, architecture, and roadmap
without exposing source code or sensitive operational information.

## Maturity Snapshot

| Layer | Public status |
| --- | --- |
| Product concept | Defined |
| Private pilot contour | Partially implemented |
| Public documentation | Released |
| Production readiness | Roadmap |
| Source code | Private |

## For Partners / Для Партнеров

This repository is open for product discussion, pilot collaboration, and
architecture review around AI-assisted accounting operations.

Этот репозиторий открыт для обсуждения пилотов, партнерств и архитектуры
AI-автоматизации бухгалтерских процессов.

- Telegram: [@a_malishev](https://t.me/a_malishev)
- GitHub: [Gudvin82](https://github.com/Gudvin82)

## Methodology

The product dossier is organized with ideas from:

- [Vibe Coding Protocols](https://github.com/Gudvin82/vibe-coding-protocols):
  intent, proof, gates, and shipped/roadmap separation.
- Strong engineering delivery practice: contracts, service boundaries,
  observable workflows, and explicit risks.
- GitHub Spec Kit style: specs, implementation plans, tasks, acceptance
  criteria, and a visible product constitution.

## Author

Created by Anatoliy Malyshev as part of a broader AI product and automation
portfolio.
