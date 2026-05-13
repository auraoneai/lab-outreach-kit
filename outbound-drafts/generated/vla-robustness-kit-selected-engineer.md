# vla-robustness-kit-selected-engineer

Project: vla-robustness-kit
Requirement: Pre-seed with one robotics research engineer familiar with VLA evals.
Channel: selected-contact
Target: robotics/VLA research engineer selected by AuraOne
Packet: templates/robotics-data-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: VLA robustness diagnostic perturbations

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
