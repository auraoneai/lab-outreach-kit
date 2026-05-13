# lerobot-quality-gates-lerobot

Project: lerobot-quality-gates
Requirement: Pre-seed with Hugging Face LeRobot maintainers or a robotics lab using LeRobot.
Channel: github-issue
Target: https://github.com/huggingface/lerobot/issues
Packet: packets/lerobot-quality-gates-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: LeRobot dataset quality gates

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
