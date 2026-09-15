# Run and stop guide

The kit maker records source-backed instructions here. This blank guide has not verified any procedure or performed any test. Apply [scope and permissions](SCOPE.md) before execution; reading a command is not authorization to run it. Actual tester attempts, setup failures, and results belong in [the version feedback record](FEEDBACK_%23%23%23%23.md), whose link must be replaced when the kit version is confirmed.

Required fields may use Unknown, Not run, Undetermined, or Not applicable with a reason. The maker supplies available guidance; testers may report gaps without filling this whole guide. Use the kit language in [README.md](README.md#kit-identity) while preserving exact commands and source evidence.

## Environment and dependencies

| Required detail | Requirement and source basis | Observed state and check basis |
| --- | --- | --- |
| Environment or platform constraints | Unknown | Unknown — not checked |
| Dependencies and required versions | Unknown | Unknown — not checked |
| Version compatibility limits | Unknown | Unknown — not checked |
| Permissions and external prerequisites | Unknown | Unknown — not checked |
| Separate authentication arrangement, if needed; no values | Unknown | Unknown — not checked |
| Current setup state | Unknown | Unknown — not checked |

Repeat dependency rows as needed. Separate required versions from versions actually observed, and date or qualify an observation when it may be stale. Record execution-time differences and setup attempts in the feedback round. No operating system, provider, toolchain, or package is required by TestRelay itself. Use Not applicable with a reason for dependency-free document or manual review.

## Methods

Add one method entry per needed check, installation, setup, run, or stop operation. For manual review, describe the action directly; omit command fields when no command is needed. Do not fill gaps with conventional-looking commands.

### Method entry

- Method identifier and purpose [required]: Unknown.
- Kind: check / install / setup / run / stop [required]: Unknown.
- Prerequisites, ownership, permissions, and effect or cost limits [required]: Unknown.
- Working directory or manual working context [required]: Unknown.
- Exact evidenced command, or manual action [required]: Unknown — no instruction established.
- Source reference and what it supports [required]: Unknown — use a permitted relative document reference or non-sensitive reference label.
- Source confirmation [required]: Unknown.
- Instruction verification [required]: Not run.
- Verification role, context, outcome, and limits [required]: Unknown.
- Applicable stop or recovery method, and its limits [required]: Unknown.
- Optional explanation: None supplied.

Source confirmation and actual instruction verification are different facts. Verification execution states are Not run, Running, Completed, or Stopped; Completed alone does not mean the method succeeded. Keep the verification outcome explicit. A later tester's execution state belongs in feedback, not in place of the maker's verification.

When documentation is inadequate, inspect only allowed dependency and version declarations, task settings, and entrypoints. Record any discovered method and its source as an unverified candidate below. Resolve needed information through the owner or verification within existing authorization and environment policy before treating the candidate as an instruction. Do not invent setup, diagnosis, stop methods, or expected results.

| Optional candidate | Source and limits | Missing information and resolving role | Verification / affected readiness |
| --- | --- | --- | --- |
| None recorded | Not applicable | Not applicable | Not run |

If a required stop method is unknown, leave it Unknown and hold the start of work that needs that stop capability. At finish, inspect existing work where possible and use known methods only for work owned by this session within permissions. Unclear ownership, cancellation authority, or stop behavior means recording remaining state and the needed role. Do not substitute blanket shared-service stops, dependency removal, global rollback, or log deletion.

## Post-copy integrity check

Use only when [existing permitted integrity artifacts](SCOPE.md#existing-integrity-context) apply. No artifact means no required new verifier or checksums. Use an evidenced method from [Methods](#methods); finding a verifier does not authorize execution.

- Authoritative reference and covered copied artifacts: Unknown — not inspected.
- Sourced method reference, working context, and execution authority: Unknown.
- Actual verification state: Not run.
- Checking role, actual context, result/mismatches, and limits: Unknown.
- Separate coverage claims for source/code bytes, added kit guides, and complete archive: Unknown — none verified.

Preserve authoritative digests; report mismatches without rewriting manifests or claiming verification succeeded. Missing authority holds only dependent verification and claims. A completed check establishes only its actual covered result, not whole-kit or archive integrity.

## Scenarios

Define only source-backed, in-scope scenarios. Refer to common methods and prerequisites above instead of duplicating them. Keep independently ready scenarios usable when others are blocked. No command is needed for a purely manual action.

### Scenario entry

- Scenario identifier [required]: Unknown.
- Purpose [required]: Unknown.
- Preconditions and applicable environment or method references [required]: Unknown.
- Actions [required]: Unknown.
- Expected result and its confirmed basis [required]: Unknown.
- Stop conditions [required]: Unknown.
- Instruction verification and limits [required]: Not run.
- Readiness and blocking information or role [required]: Not ready — scenario not defined.
- Optional notes: None supplied.

Expected results come from confirmed requirements or permitted evidence. When sources conflict or the basis is missing, hold the affected judgment; do not guess intent or declare success or failure. The tester's personal expectation remains separate in feedback. Adopting a changed expected result changes the test basis and requires a new confirmed kit version.

### Prior context to current scenarios

When [permitted prior context](SCOPE.md#prior-context) is available, add only relevant mappings. None/Unknown with its basis is sufficient otherwise; no history retrieval or extra test is required.

- Original prior reference/item and source basis: Unknown — no context established.
- Current scenario and current expected-result reference: Unknown.
- Accepted behavior or alternative, known limit, and source/confirming role: Unknown — do not infer acceptance.
- Regression/retest priority, source/confirming role, and confirmed or proposed status: Unknown.

Keep unconfirmed behavior and priorities Unknown/proposed. These mappings do not override current expected results or prove a retest ran. Preserve actual discomfort even when behavior is intended, accepted, or limited; link any needed decision through HANDOFF.

## Preparation failures and partial readiness

Record setup, version, permission, or connection failures in the actual feedback file: what was attempted, the observed error, the blocked stage, and which feature tests remain Not run. Record observed dependency versions there when available. A setup failure is not a failed feature test that never ran; a successful install is not a passing feature test.

- Ready scenarios and supporting checks [required]: Unknown.
- Blocked scenarios, missing information, and responsible role [required]: Unknown.
- Overall preparation limits [required]: Draft — no project instructions supplied.

Do not require diagnosis, repeated reproduction, packages for document-only tests, or attachments to accept a report. The [finish sequence](README.md#when-the-user-declares-testing-finished) preserves unresolved work and actual remaining jobs without promising that closing an app stops them.
