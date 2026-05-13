# a2a-contract-test-a2a-discussions

Project: a2a-contract-test
Requirement: Pre-seed with at least one A2A SDK maintainer or agent platform engineer.
Channel: github-discussion
Target: https://github.com/a2aproject/A2A/discussions
Packet: templates/agent-protocol-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: offline A2A contract profile

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
