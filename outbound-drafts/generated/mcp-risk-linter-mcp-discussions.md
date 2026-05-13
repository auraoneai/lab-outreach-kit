# mcp-risk-linter-mcp-discussions

Project: mcp-risk-linter
Requirement: Pre-seed with 2 MCP server maintainers before public announcement.
Channel: github-discussion
Target: https://github.com/modelcontextprotocol/modelcontextprotocol/discussions
Packet: packets/mcp-risk-linter-review.md
Permission to name publicly: no
Queue status: drafted

Subject:

Narrow review ask: MCP readiness linter risk taxonomy

Body:

We built `mcp-risk-linter`, a deterministic readiness linter for MCP server
repositories:

https://github.com/auraoneai/mcp-risk-linter

It checks for review prompts around risky shell execution, broad filesystem
access, network scope, auth/permission-boundary documentation, secret handling,
vague tool descriptions, and missing security docs. It is explicitly not a
security audit, CVE scanner, exploit detector, or official MCP compliance claim.

Narrow technical ask: would this taxonomy catch the MCP server risk categories
you would expect a developer tool or agent platform team to block in PR review?

Useful feedback would be:

- a missing risk category;
- a rule that is too noisy or misleading;
- wording that overclaims what a readiness linter can prove;
- remediation text that would be clearer for MCP server maintainers.

No endorsement requested or implied. A reply would only be treated as technical
feedback unless you explicitly give written permission for any public attribution.

Logging reminder:

- Do not imply endorsement, adoption, approval, certification, or partnership.
- Do not name reviewers publicly unless they explicitly grant written permission.
- After sending, update the queue/log entry from drafted to sent and record the target URL or contact channel.
