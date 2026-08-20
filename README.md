# AI Skills

Reusable, privacy-aware workflows for Codex, ChatGPT, OpenClaw, and other AI agents. This repository is the source of truth for user-maintained skills; platform-provided capabilities stay platform-managed.

Each folder contains a focused `SKILL.md` that is loaded only when its task is relevant. The point is consistent judgment without turning every prompt into an instruction dump.

## Included skills

- `writing-voice`: preserve a person's actual voice without manufacturing personality
- `openclaw`: operate and troubleshoot an OpenClaw workspace without duplicate runtimes or exposed secrets
- `mac-troubleshooting`: diagnose Mac problems from live evidence before changing anything
- `resale`: research and process resale inventory in efficient batches
- `job-search`: build application and interview materials from approved, verified source files
- `benefits-hra`: handle benefits and reimbursement workflows without putting personal data into shared systems
- `company-job-research`: research a company and role from current, attributable sources
- `interview-prep`: turn verified application and company evidence into live-use interview materials
- `sales-research`: build concise account and opportunity briefs for real commercial decisions

## Third-party skills

Third-party work lives under `third-party/` and retains its own authorship and license. It is pinned rather than silently copied when practical. See [`third-party/README.md`](third-party/README.md) for source and review details.

## Structure

```text
skill-name/
└── SKILL.md
```

The skills follow the open `SKILL.md` format used by Codex and other agent tools. They contain workflow guidance only. Credentials, transcripts, private workspace contents, case information, and client data do not belong here.

## Codex and OpenClaw

Codex discovers skills from `~/.codex/skills/<skill-name>/SKILL.md`. A local clone can be linked into that directory so Desktop Codex, Terminal Codex, and Mobile Codex sessions using the same Mac host all read the same files.

Compatible OpenClaw skills can be linked into its workspace skills directory. Links are preferred over copied instructions so fixes remain centralized.

## ChatGPT

ChatGPT does not install arbitrary GitHub `SKILL.md` packages as native skills. With GitHub connected, reference this repository and the exact skill name in the prompt. For example:

> From `bizzycore/ai-skills`, read `company-job-research/SKILL.md` and use it for this request. Load only that skill unless another one is directly required.

For sendable writing, request `writing-voice/SKILL.md`. For an application, request `job-search/SKILL.md` and `writing-voice/SKILL.md`. ChatGPT should treat the current prompt and its own safety rules as higher priority, retrieve only the relevant file, and never move private source material into GitHub.

## Platform-provided capabilities

Document, PDF, spreadsheet, GitHub, browser automation, and general research skills are already supplied by the local Codex installation. They are intentionally not copied here.

This repository is intentionally small. If an instruction does not change the agent's decisions, it probably does not need to be here.
