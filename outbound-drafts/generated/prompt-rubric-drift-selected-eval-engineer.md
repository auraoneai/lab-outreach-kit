# prompt-rubric-drift-selected-eval-engineer

Project: prompt-rubric-drift
Requirement: Pre-seed with one eval engineer who reviews prompts/rubrics in PRs.
Channel: selected-contact
Target: AI product/eval engineer selected by AuraOne
Packet: templates/ai-lab-eval-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: deterministic prompt/rubric drift PR notes

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
