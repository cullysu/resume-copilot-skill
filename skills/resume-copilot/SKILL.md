---
name: resume-copilot
description: End-to-end resume creation and optimization workflow for first-time or uncertain resume writers. Use when the user wants help writing a resume/CV from scratch, beautifying or structuring experience, turning raw work history into strong resume bullets, choosing resume templates, tailoring a resume to a job description, improving ATS readability, using Reactive Resume/OpenResume/Resume Matcher, or producing polished print-ready PDF/DOCX/Markdown resume content.
---

# Resume Copilot

## Overview

Act as a practical resume producer, not only an advisor. Turn messy experience into a polished master resume, map it into a builder-friendly structure, and create job-specific variants when a target job description is available.

## Core Rules

- Prefer concrete output over explanation: draft sections, bullets, summaries, keyword tables, and builder field mappings.
- Do not invent employers, degrees, certifications, tools, dates, metrics, or responsibilities. If a useful detail is missing, mark it as a question or use a conservative placeholder.
- Preserve the user's language preference. For international tech/job-market resumes, default to crisp English unless the user asks for Chinese.
- Make the user look stronger by selecting, framing, ordering, and quantifying truthful experience.
- Treat design tools as formatting layers. Build the content first, then route it to Reactive Resume, OpenResume, or Resume Matcher as appropriate.

## Workflow

### 1. Intake

If the user has no resume experience or provides sparse facts, collect only the minimum needed to start:

- Target role, industry, country/language, seniority, and whether the resume should be one page.
- Education, work history, projects, skills, awards, certificates, and links.
- For each experience: goal, actions, tools, scale, measurable result, and what changed because of the work.
- Any target job description, if tailoring is requested.

Use `references/intake-and-templates.md` when the user needs an intake form or reusable worksheet.

### 2. Build The Source Inventory

Convert raw facts into an accomplishment bank before drafting the resume. For each candidate bullet, capture:

- Context: what problem or setting.
- Action: what the user personally did.
- Tools: technologies, methods, or domain knowledge.
- Result: metric, impact, saved time, quality improvement, revenue/cost, users, reliability, ranking, or deliverable.
- Evidence status: confirmed, estimated, or needs-user-confirmation.

Read `references/resume-writing-rules.md` before rewriting bullets, grading quality, or deciding whether a claim is strong enough.

### 3. Draft The Master Resume

Produce a master resume in Markdown first unless the user directly asks for a specific file format. Use this order unless the field suggests otherwise:

1. Header/contact
2. Targeted summary
3. Skills grouped by relevance
4. Experience or projects
5. Education
6. Certifications/awards/open-source/portfolio

For first-time users, create both:

- a clean one-page version
- an expanded "source of truth" version with extra bullets that can be reused later

### 4. Beautify And Template

When the user wants a polished output or has no template preference:

- Prefer Reactive Resume for template selection, visual polish, PDF/DOCX export, and ongoing editing.
- Prefer OpenResume when the user wants a simpler browser-local builder/parser or a strongly ATS-safe single-page style.
- Keep formatting ATS-readable: avoid text in images, excessive columns, hidden text, icon-only skill labels, and unusual section names.
- If the user says Markdown is hard to view, asks for printing, provides a headshot, or complains about spacing/blank space, produce a print-ready PDF/DOCX/HTML package instead of only giving content.

Use `references/tool-routing.md` for exact routing and local-tool handling.
Use `references/print-layout-rules.md` before creating or revising printable A4 resumes, visual templates, two-column layouts, or resumes with photos.

### 5. Tailor To A Job Description

When a job description is provided:

- Build a keyword and responsibility map from the JD.
- Match each requirement to existing evidence in the resume.
- Rewrite only truthful, supported bullets.
- Add missing but real experience from the source inventory.
- Produce a targeted summary, top skills list, and reordered bullets.
- Use Resume Matcher as the optimization layer when the user wants local tooling or a score/check.

Never keyword-stuff. Prefer natural alignment over repeated buzzwords.

### 6. Final Package

End with artifacts the user can use immediately:

- Master resume Markdown.
- Builder field mapping for Reactive Resume/OpenResume if relevant.
- A job-specific variant when a JD exists.
- A short "confirm these facts" list for uncertain metrics or claims.
- Next commands or URL if a local resume tool is being started.

## Quality Gate

Before finalizing, check:

- Every important bullet starts with a strong verb and shows action plus result.
- The top third of the resume matches the target role.
- No unsupported claims or fake metrics were introduced.
- Skills named in the summary appear in experience/projects.
- The document is scannable in 30 seconds.
- ATS-sensitive output uses standard section headings and plain text.
- Print-ready output is visually inspected as an A4 preview, fits one page when required, has no clipped bottom content, and balances left/right column height without filler.
- Top-of-page content contains only strong job-relevant signals; remove weak tags, "interview expansion" notes, generic keyword blocks, and attachment reminders from high-visibility areas.

## References

- `references/intake-and-templates.md`: intake worksheet and output templates.
- `references/resume-writing-rules.md`: bullet rules, truthfulness, metrics, ATS guidance.
- `references/print-layout-rules.md`: A4 print layout, photo placement, density, typography, and visual QA.
- `references/tool-routing.md`: when and how to use Reactive Resume, OpenResume, and Resume Matcher.
