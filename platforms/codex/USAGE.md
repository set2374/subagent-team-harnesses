# Codex Usage

## Goal

Use these harnesses with Codex subagents while preserving durable team memory.

## Suggested pattern

1. Load the relevant team doc
2. Spawn one specialist per bounded surface
3. Give each specialist:
   - one role card
   - one task envelope
   - one write scope
4. Reuse the same specialists across rounds
5. Close specialists only when the human explicitly says to

## Recommended prompts

For each spawned Codex worker, include:

- the role card path
- the owned files/surfaces
- the exact deliverable
- the instruction not to revert other agents' work

## Memory practice

- keep a per-agent memory file based on [templates/MEMORY.md](C:/Users/set23/OneDrive%20-%20turmanlegal.com/AI%20Knowledge%20Files/subagent-team-harnesses/templates/MEMORY.md)
- update it after each meaningful slice
- when resuming an agent, feed it the memory file first

## Anti-patterns

- spawning multiple agents with overlapping write scopes
- closing agents immediately after every small task
- making the lead agent redo specialist work locally

