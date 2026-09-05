# 🧠 SECOND BRAIN V1 — OBSIDIAN-FIRST

> The operating system for knowledge, decisions, projects, learning and system evolution.

## Start here

- [[00 - Second Brain/SECOND BRAIN V1 — Canonical Architecture]]
- [[00 - Second Brain/02 — Operating Model]]
- [[00 - Second Brain/03 — Full Pass]]
- [[00 - Second Brain/04 — Authority Model]]
- [[00 - Second Brain/05 — Information Lifecycle]]
- [[00 - Second Brain/06 — Retrieval System]]
- [[00 - Second Brain/07 — QA and Verification]]
- [[00 - Second Brain/08 — Learning and Self Improvement]]
- [[00 - Second Brain/09 — Data Model]]
- [[00 - Second Brain/10 — Project Hub Template]]
- [[00 - Second Brain/11 — Research Template]]
- [[00 - Second Brain/12 — Decision Template]]
- [[00 - Second Brain/13 — Daily Capture]]
- [[00 - Second Brain/14 — System Health]]

## Four-repository system

| Repository | Role |
|---|---|
| `justinolp/Obsidian-second-brain` | Architecture and operating knowledge mirror |
| `justinolp/runtime` | Executable Runtime and mandatory evidence/completion gate |
| `justinolp/obsidian-sync` | Active `Baum/` sync/version/governance boundary |
| `justinolp/trello-conector` | Minimal Trello Power-Up iframe boundary |

## Authority model

**Interface → Runtime Gate → System Knowledge → Task Execution → System Reconciliation → Verification → Learning**

| Domain | Authority / role |
|---|---|
| Knowledge / system truth | **Obsidian / Baum** |
| Tasks / operational state | **Trello** |
| Code / versioning / repository history | **GitHub** |
| Execution oversight / evidence | **Runtime** |
| Reasoning / user interface | **ChatGPT** |
| Mobile transport | **SuperSync** |
| Mobile E2E challenge/response | **Second Brain E2E Agent + pinned device key + CI verifier** |

## Mandatory operating model

When the user says **“Benutz das Second Brain”**, the governed mode is activated:

```text
SECOND_BRAIN_FULL_PASS

RUNTIME OPERATION INIT
        ↓
SYSTEM_PRE
        ↓
TASK
        ↓
SYSTEM_POST
        ↓
RUNTIME FINAL ATTESTATION
        ↓
FINAL GATE
        ↓
TASK + SYSTEM MERGE
        ↓
COMPLETED
```

### SYSTEM_PRE — first

The System Lane runs first. It retrieves the relevant canonical Obsidian/Baum state, checks authority, invariants, capabilities, freshness, dependencies, research requirements and success contract.

### TASK — second

The Task Lane performs the user's request using the verified System_PRE state. Material side effects require observable evidence.

### SYSTEM_POST — third

The System Lane runs again. It reconciles task output against the system, captures and classifies new information, integrates affected repositories/modules, persists required changes, reads them back, verifies integrity, regression and trace, and prepares final Runtime evidence.

The Runtime enforces the phase order and must block non-canonical ordering.

## E2E transport and verification

The canonical mobile E2E boundary is:

```text
Runtime challenge
→ obsidian-sync / SuperSync
→ Android Obsidian
→ Second Brain E2E Agent
→ SuperSync return
→ GitHub read-back
→ P-256 cryptographic verifier
→ Runtime evidence
```

The E2E Agent is mobile-capable and uses the Obsidian Vault API. The repository-side verifier validates the exact challenge response against the pinned public key. A successful E2E test does not make every repository write an Android-state proof; `COMMIT ≠ MOBILE STATE` remains a hard invariant.

## Core invariants

1. One canonical authority per kind of truth.
2. Obsidian remains Knowledge/System Authority.
3. Trello remains operational and is not a second knowledge authority.
4. GitHub is code/version/history/transport boundary, not Knowledge Authority.
5. Runtime oversight cannot be silently skipped or replaced by another tool.
6. `planned != started != executed != successful != verified != persisted != completed`.
7. A claim, plan, URI, API success, commit or sync acknowledgement is not proof by itself.
8. Canonical persistence requires actual write + read-back + integrity verification.
9. Repository state does not prove Android state.
10. V1 remains on-demand; no 24/7 runtime is required.
11. The System Lane executes before and after the Task Lane.
12. Only a verified Runtime final gate may attest `COMPLETED`.
13. Device E2E identity is pinned; a changed key is a new registration and cannot silently replace the canonical identity.

## Learning

New information follows:

`CAPTURE → ATOMIZE → CLASSIFY → CANONICALIZE → LINK → PERSIST → VERIFY → LEARN`

Repeated errors become explicit rules, skills, checks or regression tests only after verification.
