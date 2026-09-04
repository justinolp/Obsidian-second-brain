# Operating Model

## Mission
Turn incoming information and requests into reliable, retrievable, actionable knowledge while continuously improving the system.

## Core loop

`Capture → Understand → Atomize → Classify → Link → Verify → Canonicalize → Persist → Retrieve → Use → Learn → Improve`

## Two-lane operation

### TASK LANE
Executes the user's actual request: understand intent, gather relevant context, research when needed, plan, execute, verify and deliver.

### SYSTEM LANE
Maintains the Second Brain: coverage, integration, persistence, QA, regression, learning, trace and architectural consistency.

The lanes run in parallel and merge at the final gate.

## Scope discipline

Load the relevant system coverage, not the entire vault blindly. Expand retrieval only when dependencies or uncertainty require it.

## State discipline

Every meaningful object should have a lifecycle state. Prefer explicit states such as `draft`, `candidate`, `verified`, `canonical`, `deprecated`, `superseded`.

## Failure discipline

A failed operation is evidence about the operation, not automatically evidence about the user's capabilities or the architecture. Diagnose → recover → retry → verify → persist the real state.
