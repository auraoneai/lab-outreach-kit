# otel-eval-bridge-otel-semconv

Project: otel-eval-bridge
Requirement: Pre-seed with one observability/eval maintainer.
Channel: github-issue
Target: https://github.com/open-telemetry/semantic-conventions/issues
Packet: templates/ai-lab-eval-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: OpenTelemetry GenAI traces to eval cases

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
