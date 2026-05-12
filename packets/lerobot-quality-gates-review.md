# Review Packet: lerobot-quality-gates

## Problem Statement

LeRobot-style datasets can look usable while hiding missing actions, inconsistent
metadata, short episodes, or timestamp alignment failures.

## Repo

`github.com/auraoneai/lerobot-quality-gates`

## Example Command

```bash
lerobot-quality-gates check examples/mock_lerobot_v3_bad --out report.md
```

## Narrow Technical Ask

Would these gates catch dataset problems you would want fixed before model
training or dataset release?

## No-Endorsement Disclaimer

This is a technical review request only. A reply does not imply endorsement,
partnership, approval, certification, adoption, or permission to use your name or
organization publicly.
