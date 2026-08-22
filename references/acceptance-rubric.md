# Acceptance Rubric

## Evidence boundary

- `runtime_evidence`: observed in the configured product path with recorded environment and steps.
- `artifact_evidence`: source, screenshot, contract, or test output inspected without completing the runtime path.
- `missing evidence`: a required behavior or state was not observable.

HTTP 200, a visible button, a passing unit test, a mock response, or a developer explanation cannot substitute for a user completing the approved task.

## Scenario contract

Each critical scenario needs persona, authority, clean precondition, start state, goal, expected completion signal, handoff/side effect, and safe reset. Include positive, empty or waiting, validation/server/permission failure, recovery, re-entry, and persistence checks where applicable.

## Verdict gates

- `pass`: all critical scenarios have runtime evidence, critical tasks complete as contracted, permission/data boundaries hold, handoffs are accepted, and no blocker remains.
- `conditional_pass`: critical scenarios complete and no safety or permission blocker remains, but only non-critical gaps have an explicit owner, workaround, and deadline.
- `fail`: any critical task, data correctness, permission isolation, handoff, recovery, or release prerequisite is blocked or contradicted.
- `not_testable`: approved contract, clean entry, or required runtime evidence is unavailable; this is not an approval.

## Severity

- `blocker`: prevents a critical task, permits unauthorized access/action, loses or duplicates consequential data, or makes recovery impossible.
- `high`: critical task is unreliable, misleading, or requires support to complete.
- `medium`: non-critical path or state has a material defect with a known workaround.
- `low`: cosmetic or low-impact inconsistency with no critical task effect.

## Independence rules

Do not use architecture, process, or UX reports as proof that the runtime satisfies them. Do not repair, reinterpret, or silently reseed while testing. If the contract is ambiguous, record the ambiguity and return it to the product owner rather than selecting a favorable interpretation.

## Handoff fields

Include `skill_name`, `skill_version`, `scope`, `input_paths`, `output_path`, `environment`, `verdict`, `blockers`, `evidence_status`, `returned_to`, and `next_action`.
