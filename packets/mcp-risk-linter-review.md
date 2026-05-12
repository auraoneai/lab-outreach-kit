# Review Packet: mcp-risk-linter

## Problem Statement

MCP servers can expose tools with destructive, data-exfiltration, or network
capabilities without enough permission metadata for reviewers to reason about
risk.

## Repo

`github.com/auraoneai/mcp-risk-linter`

## Example Command

```bash
mcp-risk-linter lint examples/risky_server.json --out report.md
```

## Narrow Technical Ask

Does the default rule set identify the MCP risk categories you would expect a
developer tool or agent platform team to block in PR review?

## No-Endorsement Disclaimer

This is a technical review request only. A reply does not imply endorsement,
partnership, approval, certification, adoption, or permission to use your name or
organization publicly.

