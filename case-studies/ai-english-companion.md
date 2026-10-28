# AI English Companion — accounting for AI usage and payments

[Profile](../README.md) · [All case studies](README.md)

**Telegram MVP · Python, aiogram, AI API and SQLite**

![AI English Companion implementation overview](../assets/ai-english-companion.png)

## Problem

An AI practice bot combines a conversation workflow with metered API usage and paid access. Replayed payment notifications must not extend access twice, and provider failures must leave the user with a clear recovery path.

## My implementation

I built the Python Telegram application, user profiles and chat history, AI API integration, usage accounting and paid-access workflows.

- **Validate payment events.** Check event identity and payment attributes before granting access.
- **Deduplicate confirmations.** Persist payment identifiers and apply access changes atomically so repeated confirmed events cannot repeatedly extend the subscription.
- **Account for AI usage.** Record usage and enforce limits in application logic.
- **Keep operations observable.** SQL reports expose usage and payment/funnel events for review.
- **Handle provider boundaries.** External AI and payment calls have distinct failure paths and user-facing recovery behavior.

## Verification in the codebase

Pytest checks cover database operations, usage limits, billing rules, payment handling, HTTP routes and regressions. Temporary SQLite databases and mocked external services make these scenarios reproducible without real charges or AI requests.

## Scope and tradeoff

This is an AI API integration, with application-level accounting and access control. Offline tests do not establish end-to-end payment-provider certification or commercial usage at scale. SQLite keeps the MVP operationally small; additional concurrency would require reviewing its write patterns and deployment model.

**Stack:** Python, aiogram, AI API, SQLite, SQL, Pytest.

This page is an implementation case study. The source repository is maintained separately. The diagram illustrates architecture rather than a live product screenshot.
