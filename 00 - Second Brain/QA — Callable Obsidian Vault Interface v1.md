# QA — Callable Obsidian Vault Interface v1

**Status:** IMPLEMENTATION GAP / E2E NOT VERIFIED
**Source:** Trello card “SYSTEM GAP CLOSURE — Callable Obsidian Vault Interface v1”

## Current architecture state

A concrete local Obsidian CLI adapter implementation and capability doctor exist in `justinolp/obsidian-sync`.

The adapter is intended to support vault targeting, search, read, create, append, move, rename, delete and Bases queries.

## Preferred bridge

Use a local process/stdio integration (MCP-compatible) rather than a public HTTP listener.

## Verification state

The implementation placeholder is considered closed, but the final host/E2E gate is **not** verified by this sync alone.

Required evidence:

1. A real local host exposes/spawns the runtime adapter.
2. The runtime performs a real Vault search/read.
3. A disposable write is performed.
4. The written content is read back.
5. Cleanup is performed and verified.
6. The resulting evidence establishes E2E verification.

Until those steps have real evidence, the state must remain:

`AVAILABLE / WIRED / EXECUTED / READ-BACK VERIFIED / E2E VERIFIED` → **E2E VERIFIED is still pending**.

## Preservation

- Obsidian remains Authority.
- Runtime remains on-demand.
- Trello remains operational.
- GitHub remains versioning/code authority.
- No 24/7 server.
- No public port.
- No second knowledge authority.
