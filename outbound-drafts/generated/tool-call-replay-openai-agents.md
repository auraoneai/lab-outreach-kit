# tool-call-replay-openai-agents

Project: tool-call-replay
Requirement: Pre-seed with 1-2 agent eval engineers.
Channel: github-issue
Target: https://github.com/openai/openai-agents-python/issues
Packet: templates/ai-lab-eval-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: turning agent traces into deterministic replay tests

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
