---
name: openclaw
description: Operate and troubleshoot Chris's OpenClaw workspace safely, with PM2 as the sole process manager and special care around duplicate runtimes and secrets.
---

# OpenClaw

## When to use

Use for OpenClaw setup, status checks, logs, configuration, updates, runtime problems, and local development in `/Users/chriscarpenter/openclaw`.

## Required inputs

- The requested outcome or observed error.
- Current workspace, Git, process, and PM2 state relevant to the issue.

## Workflow

1. Inspect the workspace and PM2 state narrowly before changing anything.
2. Check for duplicate processes, competing launch methods, ports, and stale runtime state when behavior suggests multiple instances.
3. Use PM2 for starts, stops, restarts, and process ownership; do not introduce another process manager.
4. Make the smallest in-scope change, then verify process count, status, logs, and observable behavior.

## Guardrails

- PM2 is the sole process manager.
- Never expose tokens, credentials, `.env` contents, secret values, or private configuration in commands, logs, Git, or responses.
- Do not start a second runtime to test a theory while an existing instance may still be active.
- Do not modify unrelated services, branches, or files, and do not restart or delete state without authorization.

## Output expectations

Report the observed state, action taken, verification result, and any remaining user action without dumping logs or secrets.
