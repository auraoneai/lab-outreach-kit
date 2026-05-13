# Public Review Request Drafts

These are outbound-ready drafts for the remaining v2 pre-seed review asks. They
are not sent, posted, endorsed, approved, adopted, or permissioned until an
actual outbound entry is recorded in the production outreach log.

Use each draft only in the matching public channel or a directly relevant
private contact thread. Keep the no-endorsement language intact.

## `mcp-risk-linter`

Suggested channels:

- https://github.com/modelcontextprotocol/modelcontextprotocol/discussions
- https://modelcontextprotocol-security.io/

Subject:

```text
Narrow review ask: MCP readiness linter risk taxonomy
```

Body:

```markdown
We built `mcp-risk-linter`, a deterministic readiness linter for MCP server
repositories:

https://github.com/auraoneai/mcp-risk-linter

It checks for review prompts around risky shell execution, broad filesystem
access, network scope, auth/permission-boundary documentation, secret handling,
vague tool descriptions, and missing security docs. It is explicitly not a
security audit, CVE scanner, exploit detector, or official MCP compliance claim.

Narrow technical ask: would this taxonomy catch the MCP server risk categories
you would expect a developer tool or agent platform team to block in PR review?

Useful feedback would be:

- a missing risk category;
- a rule that is too noisy or misleading;
- wording that overclaims what a readiness linter can prove;
- remediation text that would be clearer for MCP server maintainers.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `a2a-contract-test`

Suggested channels:

- https://github.com/a2aproject/A2A/discussions
- https://github.com/a2aproject/A2A/issues

Subject:

```text
Narrow review ask: offline A2A contract profile
```

Body:

```markdown
We built `a2a-contract-test`, an offline contract test kit for A2A-style agent
cards and task lifecycle behavior:

https://github.com/auraoneai/a2a-contract-test

It validates agent-card fields, declared capabilities, task state transitions,
structured payloads, malformed responses, errors, cancellation, and terminal
states. It produces Markdown/JSON reports and redacted transcript evidence.

Narrow technical ask: would this offline contract profile catch the A2A
card/task lifecycle issues an SDK maintainer would want to see before release?

Useful feedback would be:

- missing lifecycle cases;
- fields that should not be treated as required;
- better wording around non-affiliation/non-compliance claims;
- sample-agent behavior that should be changed.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `tool-call-replay`

Suggested channels:

- https://github.com/openai/openai-agents-python/issues
- https://github.com/Arize-ai/phoenix/issues

Subject:

```text
Narrow review ask: turning agent traces into deterministic replay tests
```

Body:

```markdown
We built `tool-call-replay`, a local harness that turns failed agent tool-call
traces into deterministic regression replay artifacts:

https://github.com/auraoneai/tool-call-replay

It ingests simple JSONL, OpenAI-style events, OTLP-like spans, and Phoenix-style
exports, then replays tool calls against recorded/mocked outputs without calling
live models or tools. It can emit a Markdown replay report and a generated pytest
regression test.

Narrow technical ask: does this fit how agent eval or observability teams would
turn production trace failures into repeatable regression tests?

Useful feedback would be:

- trace fields that should be preserved or redacted;
- assertions that are missing from the replay model;
- interop concerns with existing trace/export formats;
- cases where deterministic replay would create false confidence.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `agent-trace-card`

Suggested channels:

- https://github.com/Arize-ai/phoenix/issues
- https://github.com/open-telemetry/semantic-conventions/issues/2664

Subject:

```text
Narrow review ask: portable agent trace card fields
```

Body:

```markdown
We built `agent-trace-card`, a small Markdown/JSON card format for summarizing
one agent run or failure:

https://github.com/auraoneai/agent-trace-card

The card captures goal, outcome, tools used, retries, data touched,
policy/rubric checks, failure modes, human intervention, and regression status.
It is meant to be a review artifact for incidents, eval PRs, and debugging, not
an observability backend or benchmark.

Narrow technical ask: does this card capture enough evidence to discuss an agent
failure without attaching raw production logs?

Useful feedback would be:

- fields that should be added, renamed, or removed;
- privacy/redaction concerns;
- compatibility concerns with OpenTelemetry/Phoenix-style traces;
- examples that would make the format easier to review.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `lerobot-quality-gates`

Suggested channels:

- https://github.com/huggingface/lerobot/issues
- https://discuss.huggingface.co/

Subject:

```text
Narrow review ask: LeRobot dataset quality gates
```

Body:

```markdown
We built `lerobot-quality-gates`, a local CLI and GitHub Action for checking
LeRobot-style datasets before training or publication:

https://github.com/auraoneai/lerobot-quality-gates

It checks metadata completeness, episode boundaries, camera/video references,
FPS/timestamp consistency, action/state shape consistency, task labels,
intervention/recovery labels, dataset-card quality, and lightweight Hugging Face
metadata via `--hf-repo` without downloading large media files.

Narrow technical ask: would these gates catch dataset problems you would want
fixed before training or dataset release?

Useful feedback would be:

- missing LeRobot v3 metadata checks;
- rules that are too strict for real dataset workflows;
- Hugging Face dataset-card wording that should be clearer;
- examples that better match common robotics dataset failure cases.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `robot-recovery-bench`

Suggested channels:

- Robotics HIL/data-collection lab contact selected by AuraOne.
- Relevant public repository issue/discussion for a lab using HIL robot data.

Subject:

```text
Narrow review ask: robot recovery/intervention segment schema
```

Body:

```markdown
We built `robot-recovery-bench`, a small schema and metrics report for robot
human-intervention and recovery segments:

https://github.com/auraoneai/robot-recovery-bench

It measures intervention rate, recovery success rate, time-to-intervention,
failure reason, task phase, repeated-failure clusters, and whether recovery
segments are training-ready. It is a HIL/recovery data-quality diagnostic, not a
robot safety benchmark.

Narrow technical ask: would this recovery segment schema make HIL robot data
easier to audit before reuse?

Useful feedback would be:

- missing failure/recovery labels;
- fields that would be difficult to annotate consistently;
- metrics that are useful or misleading;
- compatibility concerns with LeRobot/RLDS/OpenX metadata.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `vla-robustness-kit`

Suggested channels:

- Robotics/VLA research engineer selected by AuraOne.
- Relevant public repository issue/discussion for a simulator or VLA eval project.

Subject:

```text
Narrow review ask: VLA robustness diagnostic perturbations
```

Body:

```markdown
We built `vla-robustness-kit`, a simulator-light diagnostic kit for
vision-language-action policy robustness:

https://github.com/auraoneai/vla-robustness-kit

It uses synthetic perturbations around instruction paraphrases, camera/vision
metadata, task phase ordering, embodiment metadata, and mock policy behavior.
The output is a diagnostic failure-cluster report, not a leaderboard or robot
safety claim.

Narrow technical ask: would these perturbation families be useful as a
pre-real-robot regression check?

Useful feedback would be:

- missing perturbation families;
- cases that should require simulator-backed execution;
- wording that could overclaim robustness or safety;
- metrics that would better guide follow-up data collection.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `embodiment-card`

Suggested channels:

- Robotics dataset/model maintainer selected by AuraOne.
- Relevant public dataset/model repository that publishes robot embodiment metadata.

Subject:

```text
Narrow review ask: structured embodiment card for robotics datasets/models
```

Body:

```markdown
We built `embodiment-card`, a small schema and renderer for robot datasets and
VLA model releases:

https://github.com/auraoneai/embodiment-card

It documents robot morphology, sensors, cameras, action space, coordinate
frames, control rate, teleoperation method, environment assumptions, safety
boundaries, and known limitations.

Narrow technical ask: would this make robotics dataset/model releases clearer
without turning into a heavy compliance document?

Useful feedback would be:

- fields that are missing for common robot platforms;
- fields that should be optional or renamed;
- Hugging Face README rendering concerns;
- examples that would better match real releases.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `otel-eval-bridge`

Suggested channels:

- https://github.com/open-telemetry/semantic-conventions/issues
- https://github.com/Arize-ai/phoenix/issues

Subject:

```text
Narrow review ask: OpenTelemetry GenAI traces to eval cases
```

Body:

```markdown
We built `otel-eval-bridge`, a small bridge from OpenTelemetry/Phoenix GenAI
traces to eval cases, manifests, trace cards, and regression artifacts:

https://github.com/auraoneai/otel-eval-bridge

It maps GenAI span attributes to local eval cases, preserves trace IDs, redacts
privacy-sensitive fields by default, and can attach eval results back to trace
references. It is intended as vendor-neutral glue, not a replacement for
observability platforms.

Narrow technical ask: would this preserve the trace fields an eval team needs
without overstepping OpenTelemetry semantic-convention boundaries?

Useful feedback would be:

- fields that should not be mapped into eval cases;
- privacy/redaction defaults that should change;
- missing Phoenix/OpenTelemetry examples;
- wording that should better distinguish bridge behavior from standardization.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `prompt-rubric-drift`

Suggested channels:

- AI product/eval engineer selected by AuraOne.
- Relevant public repository or discussion where prompt/rubric PR review is common.

Subject:

```text
Narrow review ask: deterministic prompt/rubric drift PR notes
```

Body:

```markdown
We built `prompt-rubric-drift`, a deterministic CLI and GitHub Action for
explaining prompt and rubric changes in pull requests:

https://github.com/auraoneai/prompt-rubric-drift

It flags changed scoring boundaries, added/deleted criteria, weight changes,
stricter or looser wording, missing examples, prompt-injection exposure, and
judge contract drift. It does not call a model.

Narrow technical ask: would this match the review workflow for teams that review
prompts and rubrics in PRs?

Useful feedback would be:

- drift categories that are missing or noisy;
- PR comment wording that would be more actionable;
- file formats that should be supported differently;
- cases where deterministic heuristics would mislead reviewers.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

## `failure-gallery`

Suggested channels:

- One agent reliability/eval reviewer selected by AuraOne.
- One robotics data/recovery reviewer selected by AuraOne.
- One devrel or open-source maintainer familiar with failure-case galleries.

Subject:

```text
Narrow review ask: synthetic agent and robotics failure gallery
```

Body:

```markdown
We built `failure-gallery`, a public synthetic gallery of agent and robotics
failure cases:

https://github.com/auraoneai/failure-gallery
https://auraoneai.github.io/failure-gallery/

Each case includes synthetic artifacts, expected findings, review labels, and a
command to reproduce a local diagnostic. The gallery is tutorial-only and does
not claim private customer data, benchmark validity, or expert-reviewed robot
safety.

Narrow technical ask: which failure cases are missing or poorly framed?

Useful feedback would be:

- synthetic cases that feel realistic or unrealistic;
- missing agent/robotics failure categories;
- wording that could imply benchmark or safety claims;
- better ways to connect cases to local diagnostic commands.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.
```

