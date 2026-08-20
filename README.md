# AI Skills

Reusable workflows I use with Codex, ChatGPT, and other AI agents.

Each folder is a small, self-contained skill. It explains when the workflow applies, what inputs it needs, how to run it, what can go wrong, and what the finished output should look like. The point is consistency without turning every task into a giant instruction manual.

## Included skills

- `writing-voice`: preserve a person's actual voice without manufacturing personality
- `openclaw`: operate and troubleshoot an OpenClaw workspace without duplicate runtimes or exposed secrets
- `mac-troubleshooting`: diagnose Mac problems from live evidence before changing anything
- `resale`: research and process resale inventory in efficient batches
- `job-search`: build application and interview materials from approved, verified source files
- `benefits-hra`: handle benefits and reimbursement workflows without putting personal data into shared systems

## Structure

```text
skill-name/
└── SKILL.md
```

The skills follow the open `SKILL.md` format used by Codex and other agent tools. They contain workflow guidance only. Credentials, transcripts, private workspace contents, case information, and client data do not belong here.

## Using the skills

Codex discovers installed skills from `~/.codex/skills/<skill-name>/SKILL.md`. ChatGPT can use compatible skills through its Skills interface or read them from a connected GitHub repository.

This repository is intentionally small. If an instruction does not change the agent's decisions, it probably does not need to be here.
