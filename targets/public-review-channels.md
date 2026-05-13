# Public Review Channels

This file lists public, non-private channels that can be used for narrow
technical review asks. Do not treat any reply as endorsement, partnership,
approval, certification, adoption, or permission to name a reviewer publicly.

## Top-Four Review Target Matrix

These are the first targets to use for the top-four v2 projects. They are
public project/community channels, not private contacts, and no outbound request
has been sent until a log entry records it.

| Project | Target 1 | Target 2 | Why this target is relevant |
| --- | --- | --- | --- |
| `mcp-risk-linter` | https://github.com/modelcontextprotocol/modelcontextprotocol/discussions | https://modelcontextprotocol-security.io/ | MCP maintainers and security-focused MCP reviewers can evaluate whether the taxonomy matches real protocol/tooling risks. |
| `lerobot-quality-gates` | https://github.com/huggingface/lerobot/issues | https://discuss.huggingface.co/ | LeRobot maintainers and Hugging Face robotics users can sanity-check dataset metadata, episode, video, action/state, and card gates. |
| `tool-call-replay` | https://github.com/openai/openai-agents-python/issues | https://github.com/Arize-ai/phoenix/issues | Agents SDK and Phoenix users are likely to care about turning failed traces into reproducible regression artifacts. |
| `agent-trace-card` | https://github.com/Arize-ai/phoenix/issues | https://github.com/open-telemetry/semantic-conventions/issues/2664 | Observability and OpenTelemetry GenAI reviewers can assess whether the trace card preserves useful failure context without over-collecting raw logs. |

## Public Source Notes

- OpenAI Agents SDK tracing docs: https://openai.github.io/openai-agents-python/ref/tracing/
- OpenAI Agents SDK issue tracker: https://github.com/openai/openai-agents-python/issues
- Arize Phoenix repository and issue tracker: https://github.com/Arize-ai/phoenix
- OpenTelemetry GenAI semantic conventions: https://opentelemetry.io/docs/specs/semconv/gen-ai/
- OpenTelemetry GenAI agentic systems issue: https://github.com/open-telemetry/semantic-conventions/issues/2664
- LeRobot repository: https://github.com/huggingface/lerobot
- LeRobot dataset docs: https://huggingface.co/docs/lerobot/lerobot-dataset-v3
- MCP community communication guidance: https://modelcontextprotocol.io/community/communication

## Agent Protocol Trust

### MCP risk review

- Packet: `packets/mcp-risk-linter-review.md`
- Primary channel: https://github.com/modelcontextprotocol/modelcontextprotocol/discussions
- Supporting community guidance:
  https://modelcontextprotocol.io/community/communication
- Suggested ask:
  "Would this MCP readiness linter catch the risk categories you would expect a
  developer tool or agent platform team to block in PR review?"

### A2A contract review

- Packet: use `templates/agent-protocol-review.md`
- Primary channel: https://github.com/a2aproject/A2A/discussions
- Fallback channel: https://github.com/a2aproject/A2A/issues
- Suggested ask:
  "Would this offline contract profile catch the A2A card/task lifecycle issues
  an SDK maintainer would want to see before release?"

## Robotics Data Quality

### LeRobot dataset quality review

- Packet: `packets/lerobot-quality-gates-review.md`
- Primary channel: https://github.com/huggingface/lerobot/issues
- Supporting channel: https://discuss.huggingface.co/
- Suggested ask:
  "Would these LeRobot-style dataset gates catch metadata, episode, video,
  action/state, and dataset-card issues you would want fixed before training or
  publishing a dataset?"

### Robot recovery/HIL review

- Packet: `packets/robot-recovery-bench-review.md`
- Primary channel: robotics lab/company contact selected by AuraOne.
- Fallback channel: relevant repository issue/discussion for a lab using HIL
  robot data.
- Suggested ask:
  "Would this recovery segment schema and report make HIL robot data easier to
  audit before reuse?"

## Observability And Trace Review

### OpenTelemetry/trace bridge review

- Packet: use `templates/ai-lab-eval-review.md`
- Primary channel: https://github.com/open-telemetry/semantic-conventions/issues
- Related public thread:
  https://github.com/open-telemetry/semantic-conventions/issues/2664
- Suggested ask:
  "Would the bridge from GenAI spans to eval cases preserve the fields you would
  expect without overstepping OpenTelemetry semantic-convention boundaries?"

### Phoenix/agent trace review

- Packet: `packets/agent-trace-card-review.md`
- Primary channel: https://github.com/Arize-ai/phoenix/issues
- Suggested ask:
  "Would this trace card capture enough evidence for an eval or observability
  maintainer to discuss an agent failure without raw production logs?"

## Logging Rule

For every actual outbound request, add an entry to
`logs/example-outreach-log.yaml` or the production outreach log with:

- date
- project
- reviewer_or_org
- channel
- packet
- status
- permission_to_name_publicly
- technical_feedback
- follow_up_owner
