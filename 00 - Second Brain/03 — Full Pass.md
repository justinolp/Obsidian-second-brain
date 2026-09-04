# SECOND_BRAIN_FULL_PASS

## 0 — Trigger / Execution Gate

Determine whether the request activates the Second Brain. If yes, execute this pass rather than improvising a partial workflow.

## 1 — Pre-flight + State Init

Initialize request state, known constraints, required authorities, dependencies, relevant system coverage and expected outcome.

## 2 — Task + System Lanes

Start TASK LANE and SYSTEM LANE together.

## 3 — Invariant / Authority / Capability Gate

Check which source is authoritative and whether the required capability is actually available and wired.

## 4 — Success Contract / DoD

Define what must be true for completion. Include verification evidence where relevant.

## 5 — Coverage

Retrieve the relevant architecture, project, dependency, skill, QA and historical context. Avoid blind full-vault loading.

## 6 — Retrieval / Research

Use existing canonical knowledge first. Research externally when freshness, uncertainty or explicit user intent requires it. Record provenance.

## 7 — Plan / Execute

Select the appropriate workflow/skill and perform the work.

## 8 — QA / Verification

Check factual correctness, system invariants, authority boundaries, output quality and side effects.

## 9 — Persistence

Atomize newly created knowledge. Classify it. Link it. Promote only verified information to canonical status.

## 10 — Read-back

Re-read the persisted target and verify that the intended state actually exists.

## 11 — Learning

Extract reusable lessons, failure modes, improvements and candidate rule/skill changes.

## 12 — Regression / Trace

Check that changes do not break established invariants. Record traceability for important changes.

## 13 — Lane Merge

Merge TASK LANE and SYSTEM LANE only after both are complete and verified.

## 14 — Final Gate

`COMPLETED` only when the success contract is satisfied and required evidence exists.
