---
name: job-search
description: Create or revise Chris's resumes, cover letters, outreach, and interview materials using approved sources, verified claims, and established document workflows.
---

# Job Search

## When to use

Use for job applications, resume tailoring, cover letters, recruiter outreach, interview preparation, and application-package validation.

## Required inputs

- The job description, company, role, and requested deliverables.
- Source files from `/Users/chriscarpenter/Library/CloudStorage/Dropbox/Job Search/`.
- For resumes, default to `/Users/chriscarpenter/Library/CloudStorage/Dropbox/Job Search/Resume Master/Chris_Carpenter_APPROVED_BASE_RESUME.docx` unless Chris provides another exact base.

## Workflow

1. Inspect the relevant source files and reuse known-good builders, templates, formatting, and validation workflows.
2. Tailor only from documented experience and verified metrics; preserve the approved layout and two-page resume length.
3. Build requested deliverables in their native format, export PDFs, and inspect rendered pages visually.
4. Run `/Users/chriscarpenter/bin/validate_application_package` for application packages and fix one failed pass before stopping.
5. Optimize interview materials for live use, normally as a polished, scannable PDF unless Chris asks for plain text.

## Guardrails

- Never invent experience, metrics, tools, industries, employers, dates, or domain expertise.
- Never select a random old or broken document when an approved source is required; stop if the correct base cannot be identified.
- Keep confidential work generic and exclude sensitive client or project details.
- Preserve Chris's natural voice by using the `writing-voice` skill when sendable prose is involved.
- Do not create extra versions, reports, or supporting documents that were not requested.

## Output expectations

Deliver only the requested files or sendable text. Application documents must be readable, visually polished, and validated before being called final.
