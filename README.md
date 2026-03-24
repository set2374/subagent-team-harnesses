# Subagent Team Harnesses

Reusable, model-agnostic subagent harnesses for engineering work. This repo is
separate from ALP and is meant to help Codex, Claude, and similar agent systems
spin up durable specialist teams without re-briefing everyone from scratch.

## What this repo is for

- Define specialist agent roles with stable responsibilities
- Preserve state across rounds with lightweight memory files
- Standardize handoffs, decision logging, and review rituals
- Give Codex and Claude the same team structure even if the spawning syntax differs

## What this repo is not

- Not a runtime dependency for ALP
- Not a replacement for your product architecture
- Not a code framework you must adopt wholesale

## License and attribution

This repository is MIT licensed. It is original harness and documentation work,
but it borrows ideas from the open-source agent-framework ecosystem, especially
VoltAgent's public examples and workflow patterns. See
[NOTICE.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/NOTICE.md).

## Initial team included

`frontend-product`

This team is designed for:

- chat-first workbenches
- three-panel legal/product workspaces
- backend thread/session integration
- research and document surfaces
- release-quality UI passes

## Structure

- [AGENTS.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/AGENTS.md)
  Global harness operating rules
- [agents/frontend-architect/AGENT.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/agents/frontend-architect/AGENT.md)
- [agents/workbench-ui-designer/AGENT.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/agents/workbench-ui-designer/AGENT.md)
- [agents/frontend-app-engineer/AGENT.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/agents/frontend-app-engineer/AGENT.md)
- [agents/backend-integration-engineer/AGENT.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/agents/backend-integration-engineer/AGENT.md)
- [agents/qa-accessibility-engineer/AGENT.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/agents/qa-accessibility-engineer/AGENT.md)
- [teams/frontend-product/TEAM.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/teams/frontend-product/TEAM.md)
- [teams/frontend-product/workflows](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/teams/frontend-product/workflows)
- [templates](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/templates)
- [platforms/codex/USAGE.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/platforms/codex/USAGE.md)
- [platforms/claude/USAGE.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/platforms/claude/USAGE.md)

## Design principles

- Durable roles beat improvised delegation
- Memory should be explicit and lightweight
- Specialists own bounded surfaces
- The lead agent integrates, but does not erase specialist context
- Agents stay open until explicitly closed

## Borrowed ideas

This repo borrows the spirit of several general agent-platform ideas:

- role cards instead of ad hoc prompts
- workflow checkpoints instead of free-form chaos
- handoff artifacts instead of oral tradition
- hook-style review points before irreversible changes

It does not copy runtime code from VoltAgent or make ALP dependent on it.

## How to use this repo

1. Pick a team in `teams/`
2. Load the relevant agent cards in `agents/`
3. Start with the team kickoff and workflow docs
4. Give each spawned subagent:
   - a bounded ownership area
   - one role card
   - one concrete deliverable
5. Persist progress in the templates here rather than relying on memory alone

## Suggested first use

For the ALP frontend:

- use the `frontend-product` team
- keep the same named specialists alive across iterations
- log decisions and carry forward each agent's memory file
