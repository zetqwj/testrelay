# TestRelay file and information mapping

This is the responsibility map for the public documents and generated kits. The [public README](README.md) provides the public entry; the [extraction guide](extraction-guide/README.md) owns the creation and packaging procedure. Each kit lives in a fresh location outside the source and public TestRelay trees.

## Public tree to generated kit

Paths in the first column start at the public root; paths in the second start at the new kit root. `FEEDBACK_<kit-version>.md` below is notation: replace the token with the owner-confirmed actual kit version, without literal angle brackets.

| Public file or directory | Generated destination | Owner → consumer; responsibility |
| --- | --- | --- |
| [README.md](README.md) | Not copied | Maintainer → everyone; entry, product boundaries. |
| [LICENSE](LICENSE) | Notice retained with distributed copied templates | Maintainer → makers/recipients; TestRelay MIT copyright and permission notice. |
| [.gitignore](.gitignore) | Not copied | Maintainer → public-repository contributors; excludes `.DS_Store` OS metadata. |
| [MAPPING.md](MAPPING.md) | Not copied | Maintainer → makers/reviewers; file ownership and change impact. |
| [extraction-guide/README.md](extraction-guide/README.md) | Not copied | Maintainer → makers/reviewers; extraction through handoff. |
| [template/README.md](template/README.md) | `README.md` | Maker → tester/session agent; kit metadata, readiness, concise start/finish flow. |
| [template/SCOPE.md](template/SCOPE.md) | `SCOPE.md` | Maker, confirmed by owner → tester/reviewer; purpose, boundaries, source baseline, permissions, inclusion list. |
| [template/RUN.md](template/RUN.md) | `RUN.md` | Maker → tester/session agent; detailed conditions, commands or manual steps, scenarios, validation status. |
| [template/FEEDBACK_####.md](template/FEEDBACK_%23%23%23%23.md) | `FEEDBACK_<kit-version>.md` | Tester → handoff owner/developer; actual attempts, experience, observations, evidence, and rounds. Others label their additions by role. |
| [template/FEEDBACK_TEMPLATE.md](template/FEEDBACK_TEMPLATE.md) | `FEEDBACK_TEMPLATE.md` | Maintainer → optional reader; short filled fictional reference only, never actual results or return evidence. |
| [template/HANDOFF.md](template/HANDOFF.md) | `HANDOFF.md` | Handoff owner or developer agent → developer; original-record links, decisions/actions, responsible roles, handoff status. |
| `template/repo/` (empty) | `repo/` | Maker → tester; independent copy of explicitly permitted program/distribution files. |
| No public counterpart | Optional `attachments/` | Recorder → permitted recipient; minimal necessary evidence linked from real feedback. |

There are nine public Markdown files and six base kit documents. The program slot is a boundary, not another document. Keep kit guides and records outside `repo/`; permitted original program documentation may remain inside it. The kit must remain readable without the public repository.

## Source information to its authoritative location

| Information or input | Kit source of truth | Transformation and downstream use |
| --- | --- | --- |
| Owner-confirmed purpose and included/excluded features | `SCOPE.md` | Record confirmation and unknowns. README gives only a concise purpose and link. |
| Read/copy scope, file inclusion, exclusions, rights, recipients, action limits | `SCOPE.md` | Distinguish reading, copying, execution, delivery, and publication. Match the inclusion list to actual files, hidden entries, link targets, and archive contents. |
| Non-sensitive source baseline and owner confirmation | `SCOPE.md` | Explain its relationship to the kit version without importing private paths, remote details, or history. |
| Existing permitted integrity manifests, digests, and verifiers | `SCOPE.md`; `RUN.md` | SCOPE owns baseline/artifact relationships, permitted integrity-file inclusion or omissions, and coverage boundaries; RUN owns sourced post-copy methods, authority, actual results or Not run, and limits. Code coverage does not prove added guides or a full archive. |
| Permitted prior-version, feedback, or change references | `SCOPE.md`; `RUN.md`; `HANDOFF.md` | SCOPE retains original references; RUN maps confirmed current behavior, alternatives, limits, and sourced regression priorities to scenarios; HANDOFF links decisions to actual items without dismissing discomfort. |
| Actual kit version | `README.md` | Use a confirmed safe kit version in the real feedback filename, headers, and handoff references. |
| Requested output language or established working language | `README.md` | Explicit request wins; otherwise established actual working language, then English. Apply to generated narrative, forms, and fictional example. Do not infer from geography, name, OS locale, or one incidental quote. |
| Filenames, commands, code, identifiers, verbatim logs/evidence | Their relevant document or `repo/` | Preserve original form across language changes. Label translated tester quotes and preserve the original; do not silently change meaning. |
| Permitted program files and runtime-required/distribution material | `repo/` | Copy explicit entries only, preserve required source/license notices, check independent writes. Missing rights or required files limit affected scenarios. |
| Dependencies, required versions, environment, setup/run/stop definitions | `RUN.md` | Capture source reference, working location, requirements, candidate/confirmed status, and actual validation separately. Allowed task definitions/configurations/entrypoints can supply unverified candidates when prose instructions are missing. |
| Confirmed requirements and expected behavior | `RUN.md` | Link scenarios to evidence; conflicting sources need a decision. Do not invent success criteria. |
| Actual installed state, setup attempts, errors, feature execution | Real versioned feedback | Record actual errors, blocked steps, and unrun features. Setup success does not establish feature success. |
| Tester actions, experience, observations, optional personal expectations | Real versioned feedback | Preserve round, role, kit version, and original account, including out-of-scenario observations. Personal expectation is not automatically an official requirement. |
| Short supporting evidence and optional attachments | Real versioned feedback; optional `attachments/` | Use minimal permitted material and relative links; record absence or limits. Fictional evidence never fills gaps. |
| Available safe runtime context and evidence correspondence | Real versioned feedback | Record actual context and map item → source/permitted locator → returned relative copy, if any, with a factual description. Runtime identifiers are not invented from item identifiers; exclude orphan attachments. |
| Actual attachment copies selected for feedback return | `HANDOFF.md` | Record return-review scope, method, result, exclusions, and limits; withhold unsafe or unreviewed copies. This is separate from initial kit review; changed copies or archives need re-review. |
| Improvement requests, hypotheses, proposed acceptance criteria | Real versioned feedback | Separate types, label role and evidence, retain unverified/proposed status. Do not rewrite observations or invent missing tester intent. |
| Optional outcome judgment against an established criterion | Real versioned feedback | Record criterion reference, judging role, and Met / Not met / Undetermined. Completion alone is not a pass. |
| Explicit finish, cleanup facts, not-run/unresolved items, remaining jobs | Real versioned feedback, current round closure | Preserve known state and limits. Link from HANDOFF instead of manufacturing stronger completion claims. |
| Needed decisions, actions, responsible roles, delivery/review status | `HANDOFF.md` | Link original round/items; summarize only when useful. Ready to send, sent, and reviewed require distinct evidence. Reviewed does not mean resolved. |
| Independently invented writing example | `FEEDBACK_TEMPLATE.md` | Retain fictional/reference labels when copying or translating. Never derive from private projects or actual feedback; never return as actual evidence. |

## Filename and language transformation

Copy all six templates to the new output before filling them. Keep five filenames unchanged. Replace `####` in the actual-record starter with the owner-confirmed kit version; it has no fixed digit count. Before committing that filename, check sensitive/unsafe characters, existing entries, real paths, and names the target filesystem treats as equivalent. The result must not collide with the example or any other file, and the actual record and example must have distinct real paths.

If the version is missing, unsafe, or colliding, seek a targeted owner decision. Do not overwrite, repurpose the fictional example, invent a version, or add an automatic suffix. Hold the affected filename finalization and kit readiness for delivery; continue independent work. A confirmed collision-free choice needs no repeated approval.

Update every generated filename reference, header, and link to the real versioned record. Encode `#` in link path components as `%23`; append an anchor only after the encoded filename and verify the anchor exists. Keep code, runnable commands, identifiers, and exact evidence unchanged by prose translation or blanket replacement. Review the selected language in metadata and throughout the generated forms and fictional reference. Public documents and templates remain English.

## Start, setup, finish, and return

| Stage | Entry → authoritative detail → saved result |
| --- | --- |
| Start | Kit README → SCOPE and version/record check → real feedback round. |
| Environment and setup | README → RUN requirements, sourced methods, validation, and stop conditions → actual attempts/errors in real feedback. |
| Test | RUN ready scenarios or authorized out-of-scenario observation → real feedback. Manual and dependency-free testing are valid. |
| Finish | README finish flow → known RUN stop methods for session-owned work → feedback closure and concise HANDOFF. No mandatory retries, diagnosis, full suite, or attachments. |
| Initial kit handoff | SCOPE recipient/inclusion limits + readiness review → all six documents and permitted `repo/` content, plus necessary permitted attachments. |
| Feedback return | Real feedback + HANDOFF + necessary permitted attachments → explicit return list and actual saved locations. Do not automatically return the program, full kit, or example. |

Explicit finish stops new tests and additional paid calls. Cleanup uses only known methods within permission for work started by the session; preserve dependencies, global state, and logs. Unknown ownership or stop methods become remaining actions. An app closing is not evidence of cleanup or delivery. A repeated finish request reports the existing closure and current known remainder; a newly requested retest adds a round without duplicating old records.

## Review changes by impact

| Change | Required review |
| --- | --- |
| Public file roles or structure | Reconcile this map, root entry, extraction guide, and all six templates; preserve nine-document scope and empty program slot. |
| Tested program, scope, procedure, or expected results | Prepare a fresh kit using an owner-confirmed new kit version; preserve the old baseline and records. Mark changed instructions not run until actually validated. |
| Feedback, analysis, closure, handoff update, or retest under the same baseline | Keep the kit version, preserve original rounds and evidence, label additions by role and basis. No automatic version increment or copied historical record required. |
| Acceptance criterion proposed during analysis | Preserve as a proposal. Adopting a changed expectation requires a new baseline/version; do not retroactively change old judgments. |
| Language, link, or filename update | Check selected language, portable relative links, encoded filename characters, actual record/example separation, and preserved original evidence. |

For an initial unused record, check blank fields and not-run status. After use, check preservation of actual observations, version/round links, grounded additions, and absence of fictional contamination; never reset it to blank. Check unresolved placeholders and permissions against scenario readiness, and keep information certainty, execution status, outcome judgment, kit readiness, and handoff status separate. A document review is not program validation or proof of delivery.
