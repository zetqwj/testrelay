# Actual feedback record

Initial state: **Not run**. No test evidence or result has been recorded. This header describes only the unused starter; update it with the actual state after use without erasing earlier content or resetting the record to blank.

This is the actual-record starter, distinct from the optional [fictional writing example](FEEDBACK_TEMPLATE.md). Rename this file using the owner-confirmed kit version before testing and update every reference in the kit. Follow the filename and collision checks in [README.md](README.md#where-to-write); never turn the example into the real record. No fictional claims or evidence belong here.

## How to record

The minimum is one round header and one item. Short or incomplete conversational feedback is accepted: the recorder preserves the original wording and marks missing fields Unknown. Do not send the tester back to complete every field before accepting or handing off the report.

Required fields accept Unknown, Not run, Undetermined, or Not applicable with a reason. These mean different things: missing information, no execution, no justified conclusion, or no applicability. A blank is never evidence of success. No real name, account, or device identifier is required.

Preserve original statements and distinguish them from independently observed evidence. Add later analysis with its author role and basis rather than editing the original statement. Write explanations in the kit language; preserve exact logs and quoted evidence, retaining originals alongside any labeled translation. Avoid collecting sensitive text or large logs to fill a field. Never copy secrets into this record.

## Round

- Round identifier [required]: Unknown — assign when recording this round.
- Kit version [required]: Unknown — match [kit identity](README.md#kit-identity) and the actual filename.
- Author or recorder role [required]: Unknown.
- Execution state [required]: Not run.
- Relevant environment differences from [RUN.md](RUN.md#environment-and-dependencies) [required]: Unknown.
- Date and elapsed time [optional]: Not supplied.

Use Not run, Running, Completed, or Stopped for execution state. Completed is not a result judgment. If items differ, state their individual execution state below. Repeat rounds for new execution under the same kit version, preserving all previous content and finish records. Give each round and item an unambiguous identifier and linkable heading when adding it.

## Item

- Item identifier, unique within this round [required]: Unknown.
- Target and action [required]: Not run — refer to a [RUN scenario](RUN.md#scenarios) or mark an observation outside a scenario; record the real action or why it did not run.
- Feeling [required]: Undetermined — no tester experience supplied.
- Observation and its limits [required]: Not run — nothing observed yet.
- Evidence [required]: None — no test attempted or statement supplied.
- Attachments [required presence or absence; files optional]: None — no evidence supplied.
- Original tester wording [when supplied]: Not supplied.

For preparation failures, the target and observation fields can capture the actual attempt, observed error, blocked stage, and feature tests Not run. Installation success and feature success stay separate. Several scenarios may share an item when they share the observation. An observation outside a scenario does not require a new scenario or authorize further actions.

Feeling describes experience, not proof of an error. Observation describes what was seen, not its inferred cause. Evidence can be a brief textual action record or screen wording without any file attachment. When only a statement exists, write “Tester statement; no independent record.” Attach only minimal permitted material via relative links; when absent, state the reason or limit. Do not assume redaction removes all sensitive metadata, or require attachments to finish.

### Evidence mapping

Use available, needed, non-sensitive context only. Missing context is acceptable; do not run more tests or retrieve history to complete these fields.

- Actual runtime correlation identifier and its source [if available and safe]: Unknown — none supplied; never derive or invent it from the item identifier.
- Relevant input characteristics and actual verification context/method [if available and safe]: Unknown — none supplied.
- Item ↔ source evidence or permitted locator ↔ returned relative copy, if any, with a factual description of what it establishes: None — no evidence supplied.

Repeat the correspondence only for actual evidence. A source can be a tester statement or permitted reference without a file. Every included attachment must map to at least one actual item; exclude orphan copies. Preserve originals, identify derived copies and relevant changes, and link only actual returned copies. Do not expose a sensitive source path or identifier; use a permitted locator or record the limit. Source evidence need not all be attached. Before return, complete [HANDOFF attachment review](HANDOFF.md#attachment-return-review); report withheld copies as exclusions, not included attachments.

### Optional interpretation and requests

- Tester expectation at the time [optional]: Not supplied.
- Improvement request and requesting role [optional]: Not supplied.
- Cause hypothesis, author role, evidence reference, and unverified limits [optional]: Not supplied.
- Acceptance criterion proposal, proposed/agreed status, and confirming role [optional]: Not supplied.
- Result judgment, judging role, and criterion reference [optional]: Undetermined — no execution or confirmed basis.

Do not invent a tester expectation absent from their reply. It may differ from RUN's expected result and is not automatically an official requirement, change request, or judgment. Keep a desired change in the request field. Hypotheses remain hypotheses. Acceptance criteria remain proposals until agreed; new criteria do not retroactively change earlier judgments. A changed test basis belongs in a new kit version.

An optional judgment is Met, Not met, or Undetermined against a stated criterion. Missing criteria or unclear judging authority leave it Undetermined. The tester need not diagnose a cause, repeat reproduction, propose a fix, or judge acceptance to submit feedback. Later fixes do not establish that a retest passed.

## Finish record

The recorder appends this to the current round when the user explicitly finishes; no new tester form is needed. Preserve earlier finish records if the user explicitly restarts in a new round.

- Declared finish intent and time [required at finish]: Unknown — no finish declaration recorded.
- Not run and unresolved items [required at finish]: Unknown.
- Existing work checked, session ownership, and inspection limits [required at finish]: Unknown.
- Cleanup actually performed, method, and permission basis [required at finish]: Not run.
- Remaining jobs or steps, current state, needed action or role, and any deferred cleanup [required at finish]: Unknown.

None and Unknown are valid when accurate. Distinguish pause, partial stop, app closure, and finish. Follow [the finish sequence](README.md#when-the-user-declares-testing-finished), then save and link this real record from [HANDOFF.md](HANDOFF.md). A repeated finish must not duplicate this round or trigger tests. Finish alone proves neither pass nor all work stopped, saving, sending, or recipient review.
