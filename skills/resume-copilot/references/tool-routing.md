# Tool Routing

## Default Recommendation

For a first-time resume writer:

1. Draft content in Markdown with this skill.
2. Put the clean master version into Reactive Resume for template polish and export.
3. Use Resume Matcher only after a target job description exists.

## Reactive Resume

Use for:

- From-scratch resume building.
- Visual templates and polished PDF/DOCX export.
- Long-term editing and maintaining multiple versions.
- Users who care about presentation and do not yet have a template.

Local handling:

- If `D:\下载\resume-tools\reactive-resume` exists, inspect its README/package files and follow official startup instructions.
- If it is not installed, clone from `https://github.com/AmruthPillai/Reactive-Resume`.
- Do not configure AI provider keys unless the user explicitly provides them.

Content handoff:

- Paste the drafted Summary into the summary/headline fields.
- Use Experience for paid/professional roles.
- Use Projects for personal, academic, maker, open-source, or portfolio work.
- Keep bullet lists concise: usually 2-5 bullets per role/project.

## OpenResume

Use for:

- A simpler local/browser resume builder.
- ATS-readable single-page output.
- Importing/parsing an existing PDF.
- Users who prefer minimal setup.

If choosing between OpenResume and Reactive Resume for a beginner, prefer Reactive Resume when visual polish matters and OpenResume when simplicity/ATS parsing matters more.

## Resume Matcher

Use for:

- Tailoring an existing master resume to a specific job description.
- Keyword gap analysis.
- AI suggestions for per-application resume variants.
- Cover letter generation when supported.

Local handling:

- If `D:\下载\resume-tools\resume-matcher` exists, inspect `README.md` and `SETUP*.md` before starting.
- The project may require Python 3.13+, Node.js 22+, uv, and optional local or API LLM configuration.
- If AI configuration is missing, still use it for available non-secret setup and document what remains.

## Privacy

Do not upload the user's resume or personal information to hosted services unless the user explicitly asks. Prefer local tools for sensitive drafts. Redact phone, address, email, and IDs in screenshots or examples unless the user wants final production content.

## When Tools Are Unavailable

If a tool cannot run, continue with the skill workflow:

- Produce Markdown master resume.
- Produce builder field mapping.
- Produce a JD match table manually.
- Provide exact blocked prerequisite and next command.
