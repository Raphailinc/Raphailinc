# Ping — confirm, persist and deliver a reminder

[Profile](../README.md) · [All case studies](README.md)

**Personal product · Python, FastAPI, PostgreSQL and React/TypeScript**

## Problem

A forwarded message may contain an ambiguous date or incomplete context. Saving an inferred reminder without confirmation risks notifying the user at the wrong time. Keeping schedules only in process memory would also lose them after a restart.

## My implementation

I built the initial Telegram reminder workflow and developed it into a web workspace with a separate FastAPI/React client.

1. **Capture.** Accept a forwarded message or reminder request.
2. **Confirm.** Present the proposed text and time for the user to correct before saving.
3. **Persist.** Store the reminder in PostgreSQL so it survives application restarts.
4. **Deliver.** A worker processes due reminders and supports completing or postponing them.

When optional AI extraction is unavailable, the fallback asks for missing information. The web workspace adds owner-scoped tasks, notes, habits and calendar views. Docker Compose and backup/restore scripts support deployment and recovery work.

## Verification in the codebase

The repository contains unit and integration checks for reminder behavior, ownership, web API flows and recovery tooling. Some web/database scenarios require a running PostgreSQL instance. Deployment documentation distinguishes the limited pilot from locally developed functionality.

## Scope and tradeoff

Confirmation adds an interaction but gives the user control over ambiguous input. The initial scheduler is a simple persisted worker, with no claim of distributed exactly-once delivery. The product continues to evolve; integrations and workspace features have separate readiness constraints.

**Stack:** Python, FastAPI, PostgreSQL, Docker Compose, React, TypeScript, Pytest.

This page is an implementation case study. The source repository is maintained separately.
