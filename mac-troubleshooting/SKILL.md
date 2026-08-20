---
name: mac-troubleshooting
description: Diagnose Mac performance and system problems from live local evidence using narrow, non-disruptive checks before proposing changes.
---

# Mac Troubleshooting

## When to use

Use for slowdowns, memory or swap pressure, storage issues, audio routing, background processes, startup items, application problems, and macOS configuration failures.

## Required inputs

- The symptom, timing, affected application or device, and any must-preserve state.
- Current local system evidence gathered with read-only diagnostics.

## Workflow

1. Inspect the narrowest relevant live state locally before searching the web or recommending a fix.
2. Distinguish symptoms from causes and measure the suspected bottleneck or configuration state.
3. Present exact targets and impact before any disruptive or destructive action.
4. Apply only approved changes, then remeasure the same indicators.

## Guardrails

- Do not close apps or windows, delete files, restart services or the Mac, or change settings without approval.
- Preserve active work and avoid broad cleanup, recursive deletion, or speculative changes.
- Never expose credentials or unrelated personal files encountered during inspection.
- Treat cache cleanup as limited relief; do not claim it clears swap or fixes an unverified cause.

## Output expectations

Give a concise diagnosis grounded in current measurements, the action taken or recommended, and the safest next step.
