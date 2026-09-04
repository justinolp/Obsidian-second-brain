# QA — Obsidian Access Interface Audit — 2026-09-04

**Status:** CANONICAL QA RECORD
**Source:** Trello card “2026-09-04 — Obsidian Access Interface & Architecture Audit”

## Access recovery rule

If a run, tool, or error reports “no access to Obsidian”, treat this as an Access/Integration-Failure signal first. Do not persist it as a permanent capability statement about the user.

The workflow must:

1. inspect the Obsidian interface/integration;
2. reinitialize or restore the access path;
3. retry access;
4. read back the Obsidian target state;
5. only then continue with vault-level work.

Stop only at a technically hard, demonstrable boundary.

## Truth model

`AVAILABLE → WIRED → EXECUTED → READ-BACK VERIFIED → E2E VERIFIED`

“No access” is valid only as a concrete temporary/technical status backed by an observed failure.

## Architecture audit findings

- Obsidian Authority model preserved.
- Full-Pass preserved.
- Knowledge pipeline, linking, retrieval, QA, persistence and learning remain integrated.
- Atomicity is the guiding principle.
- Semantic links and MOC/index structures are distinct.
- Properties should be controlled and standardized.
- Bases are suitable for structured views.
- Retrieval should combine Search + Properties + Backlinks + Outgoing Links.
- Project Hubs are supported.
- PARA is an organizational dimension only.
- Obsidian URI is suitable for cross-app automation.
- Canonical rules require verification + regression.

## Success contract

Obsidian access is handled correctly, actual access is verified through read-back, vault findings are based on real read-back, and no false permanent “no access” claim is persisted.
