# SECOND BRAIN V1 — Canonical Architecture

**Status:** CANONICAL  
**Last reconciled:** 2026-09-05  
**Authority:** Obsidian / Baum  
**Engineering mirror:** `justinolp/obsidian-sync`  
**Runtime implementation:** `justinolp/runtime`

## 1. Authority model

| Domain | Authority / role |
|---|---|
| Knowledge & system truth | **Obsidian / Baum** |
| Operational tasks / control state | **Trello** |
| Code, versioning, repository history | **GitHub** |
| Execution oversight / evidence gate | **Runtime** |
| User-facing reasoning / interface | **ChatGPT** |
| GitHub ↔ Android Obsidian transport | **SuperSync** |
| Local Obsidian actuation | **Advanced URI / supported local adapter** |

GitHub is not the Knowledge Authority. Trello is not a second knowledge authority. Runtime does not replace either authority; it enforces the evidence and lifecycle contracts between them.

## 2. Four-repository system boundary

- `justinolp/runtime` — executable Runtime, deterministic completion gate, orchestration, adapters, persistence and trace.
- `justinolp/Obsidian-second-brain` — canonical human-readable Second Brain architecture and operating knowledge.
- `justinolp/obsidian-sync` — active `Baum/` transport/version mirror plus repository-side governance and Runtime evidence checks.
- `justinolp/trello-conector` — minimal Trello Power-Up iframe boundary; it is not Runtime and does not become a knowledge store.

These repositories are complementary, not competing authorities. Cross-repository changes must preserve the authority map and be reconciled before canonical promotion.

## 3. Canonical execution route

`TRIGGER → EXECUTION GATE → PRE-FLIGHT + STATE INIT → RUNTIME OPERATION INIT → TASK + SYSTEM LANES → AUTHORITY / CAPABILITY → SUCCESS CONTRACT / DoD → RELEVANT COVERAGE → OBSIDIAN RETRIEVAL → RESEARCH WHEN REQUIRED → PLAN → EXECUTE → RUNTIME OVERSIGHT → QA / VERIFICATION → PERSISTENCE → READ-BACK → INTEGRITY → DEPENDENCIES → REGRESSION → LEARNING → TRACE → RUNTIME VERDICT → FINAL GATE → LANE MERGE → COMPLETED`

The Runtime is a mandatory control point, not an after-the-fact report. If Runtime participation or required evidence is missing, the operation remains blocked/unverified and cannot be promoted to `COMPLETED`.

## 4. Truth-state model

`INTENDED → ATTEMPTED → SUCCEEDED → VERIFIED → PERSISTED`

`REGRESSED` invalidates a previously verified state when later evidence contradicts it.

For capability and integration state:

`DOCUMENTED → AVAILABLE → WIRED → EXECUTED → READ-BACK VERIFIED → E2E VERIFIED → ACTIVE`

For cross-interface persistence, a commit, API success, generated URI, sync acknowledgement or assistant statement is not destination proof by itself.

## 5. Persistence / no silent data loss

No information is considered permanently saved, integrated, `ACTIVE` or `COMPLETED` until the authoritative Obsidian target has actually been written, read back and integrity-verified.

Repository state proves repository state. It does not automatically prove Android Obsidian state. Device/E2E status must remain separately evidence-scoped.

## 6. Non-bypass invariant

The assistant may not bypass Runtime by omission, wording, alternate tooling, route changes, manual instructions, self-attestation, stale state, overwrite, deletion of evidence or a success declaration.

Changing from GitHub to URI, SuperSync, Trello or another adapter does not remove the Runtime obligation. If the required Runtime actuator is unavailable, the truth state is downgraded rather than simulated.

## 7. Mobile / sync boundary

Canonical Android vault path: `/storage/emulated/0/Documents/Baum`  
Repository sync root: `Baum/`

`ChatGPT → Full Pass → Runtime → GitHub → SuperSync → Android Obsidian`

The historical path `Second brain/SECOND_BRAIN_V1_Obsidian/SECOND_BRAIN` is not an active runtime, sync, URI, QA or completion target.

## 8. Research and learning

Canonical knowledge is retrieved before invention. External research is used when freshness, uncertainty or explicit user intent requires it. New information follows:

`CAPTURE → ATOMIZE → CLASSIFY → CANONICALIZE → LINK → PERSIST → VERIFY → LEARN`

Repeated errors become explicit rules, skills, checks or regression tests.

## 9. Completion invariant

`COMPLETED` is a system attestation, not conversational wording. It requires:

- applicable TASK and SYSTEM lanes executed and verified;
- Runtime oversight executed with a valid final verdict;
- required persistence/read-back/integrity evidence;
- applicable regression and trace checks;
- no unresolved mandatory blocker.

Only a Runtime `PASS` satisfies the Runtime portion of the final gate. `PASS_WITH_UNVERIFIED_EXTERNAL_STATE` is not full completion.
