# Resume Copilot Skill

A privacy-conscious Codex skill for turning rough career notes into polished, job-targeted resumes.

This repository contains only a generic skill workflow. It does not include personal resumes, contact details, school records, screenshots, or private user data.

## What It Helps With

- Build a resume from sparse or messy notes.
- Turn raw experience into truthful, stronger resume bullets.
- Choose a template based on target role, seniority, and output format.
- Tailor a resume to a job description without keyword stuffing.
- Prepare print-ready or ATS-readable resume content.
- Balance A4 print layouts, including photo placement, spacing, font sizing, and left/right column density.
- Route work to local resume tools when useful.

## Install

After this repository is published, install the skill with Codex's skill installer from:

```powershell
python "C:\Users\cully\.codex\skills\.system\skill-installer\scripts\install-skill-from-github.py" --repo cullysu/resume-copilot-skill --path skills/resume-copilot
```

Restart Codex after installation so the new skill is discovered.

## Repository Layout

```text
skills/resume-copilot/
  SKILL.md
  references/
    intake-and-templates.md
    print-layout-rules.md
    resume-writing-rules.md
    tool-routing.md
```

## Privacy Boundary

Use this skill with local files for sensitive drafts. Do not publish a user's resume, phone number, email, private education records, screenshots, or job-search materials unless the user explicitly requests that exact publication.
