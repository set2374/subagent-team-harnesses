# Subagent Harness Rules

These instructions apply inside this repository.

## Goal

Create reusable harnesses for persistent specialist teams. Favor portability
across agent platforms over platform-specific tricks.

## Core operating rules

1. Specialists own bounded surfaces.
2. Handoffs are written, not implied.
3. The lead agent integrates work but does not overwrite specialist memory.
4. Keep persistent agents alive until the human explicitly says to close them.
5. Prefer lightweight artifacts over sprawling process.

## Required artifacts

Every team should have:

- one team brief
- one role card per specialist
- one workflow map
- one handoff template
- one memory template

## Writing style

- plain markdown
- short sections
- direct language
- no model-specific jargon unless isolated in platform docs

## Role card requirements

Each agent card should state:

- mission
- scope
- explicit non-goals
- preferred inputs
- required outputs
- memory rules
- collaboration rules

## Memory rules

- Each persistent agent should maintain a small `MEMORY.md` beside its role card
  or in a project-local memory location.
- Memory should capture:
  - decisions
  - stable assumptions
  - unresolved questions
  - owned files or surfaces
- Do not turn memory into a transcript dump.

## Closure rule

Do not close persistent agents automatically after a deliverable lands.
Close them only when:

- the human explicitly requests closure, or
- the team is being intentionally reset.

