# Workflow 03: API and State Wiring

## Goal

Replace mock seams with stable thread- and state-aware backend integration.

## Checklist

- define send-message endpoint
- define thread continuity key
- define list/hydrate thread endpoints
- keep auth and token handling explicit
- add contract tests
- keep notebook and workbench APIs deferred unless needed now

## Exit condition

The frontend can send a message, continue a thread, and restore prior thread
state after refresh.

