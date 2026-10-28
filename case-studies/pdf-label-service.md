# PDF Label Service — transactional code reservation

[Profile](../README.md) · [All case studies](README.md)

**Local MVP · FastAPI, SQLite and PDF processing**

![PDF Label Service implementation overview](../assets/pdf-label-service.png)

## Problem

A label-generation tool must avoid printing the same supplied marking code twice. A crash after a PDF has been written is especially awkward: automatically returning those codes to the available pool could allow a second batch to reuse them.

## My implementation

I built a local FastAPI service that takes PDF label templates and previously issued code PDFs, assembles output labels and records each batch in SQLite.

- **Reserve before export.** Code allocation happens inside an immediate SQLite transaction, with checks against previous reservations and use.
- **Explicit lifecycle.** A batch moves through `RESERVED → EXPORTING → SUCCESS` rather than relying on the presence of an output file alone.
- **Conservative recovery.** Interrupted work with a possible output file becomes `REQUIRES_REVIEW`. An operator explicitly resolves the uncertain batch before its codes can be released.
- **Rollback on insufficient inventory.** A failed reservation leaves the available-code pool consistent.
- **PDF object preservation.** The pipeline places source Data Matrix objects into the output PDF rather than decoding and redrawing their contents.

## Verification in the codebase

Tests cover committed-code reuse, rollback when inventory is insufficient, interrupted-export recovery, and the API/PDF workflow. Temporary databases and generated fixtures isolate checks from actual production batches.

## Scope and tradeoff

SQLite suits the single-machine workflow and keeps deployment local. The MVP uses codes supplied by the operator; it does not issue codes or integrate with the national marking system. Physical scan quality still depends on the printer, label material and agreed print geometry. Windows/CorelDRAW conversion requires its own acceptance checks.

**Stack:** Python, FastAPI, SQLite, pypdf, unittest.

This page is an implementation case study. The source repository is maintained separately. The diagram illustrates architecture rather than a live product screenshot.
