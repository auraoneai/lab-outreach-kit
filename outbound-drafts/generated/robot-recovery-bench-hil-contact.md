# robot-recovery-bench-hil-contact

Project: robot-recovery-bench
Requirement: Pre-seed with one robotics HIL/data collection team.
Channel: selected-contact
Target: robotics HIL/data-collection lab contact selected by AuraOne
Packet: packets/robot-recovery-bench-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: robot recovery/intervention segment schema

Body:

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

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
