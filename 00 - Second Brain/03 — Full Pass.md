# SECOND_BRAIN_FULL_PASS

## Purpose

Every relevant Second Brain request runs through this controlled pass. It is not a suggestion list: mandatory gates cannot be silently skipped.

## 0 — Trigger / Execution Gate

Determine whether the request activates the Second Brain. If yes, initialize a governed operation. If the required Runtime control point cannot participate, do not claim completion.

## 1 — Pre-flight + State Init

Initialize request state, known constraints, required authorities, dependencies, relevant system coverage, target state and expected outcome.

## 2 — Runtime Operation Init

Create a stable operation identity and success contract. The Runtime must receive/observe the operation lifecycle and remain attached until the final verdict.

## 3 — Task + System Lanes

Start **TASK LANE** and **SYSTEM LANE** together. TASK handles the user's objective. SYSTEM handles relevant coverage, maintenance, integration, persistence, QA, regression, learning and trace.

## 4 — Invariant / Authority / Capability Gate

Resolve authority before execution. Check capability rather than assuming it. Conflicts and unavailable actuators block rather than being silently substituted.

Authority precedence:

1. platform/system safety and hard capability constraints
2. explicit current user instruction
3. active canonical Obsidian controls
4. current verified state/context
5. high-quality external evidence
6. historical/uncertain/superseded records

## 5 — Success Contract / DoD

Define what must be true for success. Include observable verification evidence and persistence requirements where applicable.

## 6 — Relevant Coverage

Retrieve only the relevant architecture, project, dependency, skill, QA and historical context. Do not blindly load the whole vault.

## 7 — Retrieval / Research

Use canonical Obsidian knowledge first. Use external research when freshness, uncertainty or explicit user intent requires it. Record provenance for material external evidence.

## 8 — Plan / Execute

Select the applicable workflow/skill and perform the work through governed adapters. Distinguish `INTENDED`, `ATTEMPTED`, `SUCCEEDED` and `VERIFIED`.

## 9 — Runtime Oversight

The Runtime independently checks machine-verifiable execution evidence, target state, authority, freshness, invariants, persistence, read-back, integrity, dependencies, regression and trace. An assistant statement is never sufficient as sole execution proof.

## 10 — QA / Verification

Check factual correctness, authority boundaries, system invariants, output quality and side effects. Failed or contradictory evidence is not promoted to success.

## 11 — Persistence / Integration

Atomize newly created knowledge. Classify, canonicalize, link and persist it in the authoritative target. For writes, use current-state/conditional-write protection where supported.

## 12 — Read-back / Integrity

Re-read the actual persisted target. Verify the intended content/state and integrity. A successful write or commit alone is insufficient.

## 13 — Learning

Extract reusable lessons, failure modes, improvements and candidate rule/skill changes. Promote candidates only after verification and regression.

## 14 — Regression / Trace

Check that changes do not break established invariants, routes, dependencies or known canaries. Record a stable operation trace for important changes.

## 15 — Runtime Verdict

Allowed outcomes include `PASS`, `PASS_WITH_UNVERIFIED_EXTERNAL_STATE`, `BLOCKED`, `FAIL` and `REGRESSED`. Only `PASS` satisfies the Runtime portion of the final gate.

## 16 — Lane Merge

Merge TASK and SYSTEM lanes only after all applicable required gates and evidence are verified.

## 17 — Final Gate

`COMPLETED` only when the success contract is satisfied, required evidence exists, persistence/read-back is verified where applicable, no mandatory blocker remains and the Runtime has returned `PASS`.

### Hard distinction

`planned != started != executed != successful != verified != persisted != completed`

Missing Runtime evidence is a control failure, not permission to continue as though the pass succeeded.
