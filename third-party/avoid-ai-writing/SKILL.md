---
name: avoid-ai-writing
description: Audit or revise prose for common AI-writing patterns using the pinned upstream skill while preserving the user's own voice rules.
license: MIT
metadata:
  author: Conor Bronsdon
  upstream: https://github.com/conorbronsdon/avoid-ai-writing
  integration: compatibility-adapter
  reviewed: 2026-08-20
---

# Avoid AI Writing

When the user requests an AI-pattern audit or rewrite, read `upstream/SKILL.md` completely and apply the relevant mode only. The installed adapter provides `upstream` as a link to the pinned source.

Use `writing-voice` as the authority for the user's actual personality, wording preferences, and sendable output. Treat upstream pattern flags as editing signals, not proof of authorship, and do not replace specific human phrasing with generic polish.

Do not run upstream scripts unless the user requests a deterministic check and the script has been re-inspected for the current pinned revision. Return only the requested audit or revised text unless commentary is requested.
