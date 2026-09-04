# QA and Verification

## Verification levels

- **L0 — Unchecked:** captured but not validated.
- **L1 — Plausible:** internally coherent, evidence incomplete.
- **L2 — Verified:** supported by appropriate evidence.
- **L3 — Read-back verified:** persisted state was re-read and matches intent.
- **L4 — E2E verified:** full integration path demonstrated.

## QA gates

### Content QA
Accuracy, completeness, source quality, ambiguity and contradictions.

### System QA
Invariants, authority boundaries, dependencies, lifecycle state and compatibility.

### Integration QA
Adapter availability, execution, persistence, read-back and external side effects.

### Regression QA
Previously working workflows remain compatible after changes.

## Hard rule
Never mark a state verified merely because an operation was requested or code was written. Verification requires observable evidence.
