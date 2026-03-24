# Claude Usage

## Goal

Use the same harness with Claude's stateful subagents and persistent teams.

## Suggested pattern

1. Start with the team doc and the relevant workflow file
2. Create named specialists that map to the role cards in `agents/`
3. Give each Claude subagent:
   - one role card
   - one bounded task envelope
   - one memory file to maintain
4. Reuse the same named specialists across sessions when possible
5. Close them only when intentionally winding the team down

## What to preserve between rounds

- role card
- last handoff
- memory file
- owned surfaces
- unresolved blockers

## Good Claude-team habits

- keep handoffs short and structured
- use written memory instead of assuming long conversational recall
- keep one coordinator responsible for integration

## Anti-patterns

- letting all subagents edit the same area
- asking every specialist to solve the whole problem
- wiping team state by recreating everyone each round

