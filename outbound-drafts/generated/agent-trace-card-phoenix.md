# agent-trace-card-phoenix

Project: agent-trace-card
Requirement: Pre-seed with one eval/observability maintainer.
Channel: github-issue
Target: https://github.com/Arize-ai/phoenix/issues
Packet: packets/agent-trace-card-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: portable agent trace card fields

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
