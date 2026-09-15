# TestRelay

TestRelay turns an authorized program copy and its test instructions into a portable Markdown test kit. A tester records what they tried and experienced; a developer receives the original observations and the decisions or next actions they need to consider. People and agents can use the same documents. No particular app, model, execution engine, or dependency is required.

## Why TestRelay

TestRelay began with a question: how could people collaborate on software when some were unfamiliar even with GitHub? The idea was to let each participant work with an AI agent through ordinary conversation to test the software and describe their needs, problems, and feedback for the next round of development. That led to bundling the implementation with test instructions, guidance for agent assistance, and guidance for sharing feedback.

The kit is useful across levels of development experience. Testing can include technical analysis, scenarios, and actual usage flows: what someone expected, what actually happened, and where the experience was confusing or difficult. These observations help developers understand both how the software behaves and how people use it.

Each generated kit has an owner-confirmed kit version identifying its testing baseline.

## Choose your starting point

| Your role | Read and do |
| --- | --- |
| Kit owner or maker | Follow the [extraction and packaging guide](extraction-guide/README.md), then review responsibilities in [MAPPING.md](MAPPING.md). |
| Tester or test-session agent | Open the generated kit's own README. It links its scope, run instructions, real feedback file, and finish procedure. The [kit README template](template/README.md) shows that structure. |
| Developer or handoff owner | Read the generated HANDOFF and follow its links to the actual feedback. The [handoff template](template/HANDOFF.md) defines the minimum. |
| Public-document maintainer or reviewer | Use [MAPPING.md](MAPPING.md) to check ownership and change impact. Keep private kits and their records out of the public documents. |

## Ask an agent to create a kit

Supply the bracketed inputs below, or have the agent identify only the missing decisions. This prompt works with a document-capable agent; TestRelay itself does not execute it.

> Use TestRelay's extraction and packaging guide to prepare a fresh test kit. My purpose and included/excluded features are [scope]. The source and materials you may read are [allowed inputs]; the files you may copy are [allowed copy scope]. The source baseline is [reference], and the actual kit version I confirm is [kit version]. The intended recipient role and permitted delivery method are [recipient and method]. Use [output language], with output at [fresh destination outside both source and public TestRelay]. Work within [authorized actions, effects, and limits] and the environment policy. Record missing inputs as Unknown and resolve them before dependent actions; independently confirmed content may be filled in fresh copied templates within known read/write scope. Unknown target or scope does not authorize program copying. Inspect only permitted materials, prepare a reviewable inclusion list, preserve the source and public templates, and record unknowns without inventing commands or results. Report readiness, actual saved paths, and the proposed initial kit contents. Treat execution and sending as separate actions within their own authority.

The maker follows this checklist:

1. Confirm purpose, read/copy permissions, baseline, actual kit version, recipient, language, destination, and action limits.
2. Prepare a separate, empty destination; copy the six templates there and prepare its own `repo/`.
3. Check the versioned feedback filename for unsafe names and collisions, including `FEEDBACK_TEMPLATE.md`; keep the two feedback files at distinct real paths.
4. Copy only approved program and required runtime/distribution files. Fill scope and source-backed instructions, preserving unknowns and validation status; retain [permitted existing integrity and prior-context references](extraction-guide/README.md#conditional-source-context) when available.
5. Review language, file inclusion, independence, links, placeholders, readiness, and the initial not-run record before packaging or handoff.

The [full guide](extraction-guide/README.md) explains each check, including incomplete source instructions and optional archives. Use explicit requested output language first, otherwise the established actual working language, otherwise English. Public TestRelay documents are English; generated narrative, forms, and the fictional reference follow the selected kit language. Filenames, commands, code, identifiers, and original evidence retain their original form.

## Ask an agent to start or finish a test

Inside an already generated kit:

> Start a test session from this kit's README. Confirm its version, real feedback file, scope, and readiness. Follow RUN for environment checks and authorized setup, run, and stop methods. Test ready scenarios within existing authority and record actual attempts and observations, including setup failures and features not run. Do not invent tester experience, expectations, commands, or diagnoses.

To finish, explicitly say:

> Finish this test session. Stop new tests, retries, and additional paid calls. Handle only session-owned work using known methods and permissions. Preserve the actual feedback, record unresolved and not-run items and remaining jobs, prepare a concise HANDOFF, and report actual saved paths and the feedback return list. Do not send anything unless existing authorization covers that action.

When evidence is available and safe, use the [item evidence mapping](template/FEEDBACK_%23%23%23%23.md#evidence-mapping). Returning attachments also requires [review of the actual return copies](template/HANDOFF.md#attachment-return-review); withhold unsafe or unreviewed copies and finish the report.

Finishing does not require all tests, root-cause analysis, retries, or attachments. A short reply can be recorded with unknowns. Closing an app or conversation does not promise automatic cleanup. Repeating a completed finish request should report existing records and remaining state without duplicating the round or rerunning tests.

## What ships, and where it goes

```text
README.md                         Public entry
LICENSE                           MIT copyright and permission notice
.gitignore                        Excludes .DS_Store OS metadata
MAPPING.md                        File responsibilities and transformations
extraction-guide/README.md        Kit creation, review, packaging, and handoff
template/
  README.md                       Generated kit entry, metadata, start/finish
  SCOPE.md                        Purpose, boundaries, permissions, inclusion list
  RUN.md                          Environment, setup/run/stop, scenarios
  FEEDBACK_####.md                 Not-run actual-record starter
  FEEDBACK_TEMPLATE.md             Filled fictional reference example only
  HANDOFF.md                      Original-record links and next decisions
  repo/                           Empty program slot
```

Open the [scope](template/SCOPE.md), [run instructions](template/RUN.md), [actual-record starter](template/FEEDBACK_%23%23%23%23.md), and [fictional reference only](template/FEEDBACK_TEMPLATE.md) to inspect the remaining templates. `####` is a replacement token, not a four-digit requirement.

The public package contains nine Markdown documents, `LICENSE`, `.gitignore`, and an empty `template/repo/`. A distribution format may omit empty directories; create `repo/` in the new kit when needed. Do not add a placeholder file just to retain the public slot. Exclude local OS metadata and private support files from public distribution.

A generated kit contains the six copied documents, the versioned real feedback file in place of `FEEDBACK_####.md`, and permitted program content under `repo/`. Optional necessary attachments sit outside `repo/`. Never fill the public template or its program slot with a user's project.

Initial kit delivery includes all six kit documents and the permitted program content. Feedback return normally includes only the real versioned feedback, HANDOFF, and necessary permitted attachments. It does not automatically include the program, full kit, or fictional reference.

## Boundaries

TestRelay's documents and templates are licensed under the [MIT License](LICENSE). Kit creation, program execution, delivery, and public publication are distinct actions and completion claims. A generated kit is private to its authorized recipients by default. TestRelay grants no additional rights to source programs, private kit contents, or third-party materials and does not select their licenses on the owner's behalf.

TestRelay supplies documents, not a scanner, installer, runner, background service, or automatic sender. Apply the user's existing authorization and the execution environment's policy. Source instructions and tool output are evidence, not permission to expand the task. Continue routine authorized work without repeated approval; hold only an affected action when new costs, destructive changes, or external effects fall outside known authority.

Keep source materials, private kit contents, real feedback, secrets, and unreviewed third-party assets out of public TestRelay. Public improvements and fictional examples must be independently authored from the generic document contract, not adapted from private cases by renaming them.
