# Print Layout Rules

Use this when producing a resume the user will print, hand to HR, or review as PDF/DOCX rather than Markdown.

## Artifact Contract

When the user needs a printable resume, produce:

- PDF as the primary print artifact.
- DOCX as the editable artifact when possible.
- HTML or image preview for visual review when generated from HTML/CSS.

Do not stop at Markdown if the user says they cannot view Markdown or needs a document to print.

## A4 Layout Defaults

For Chinese one-page resumes, start with:

- A4 portrait, zero browser header/footer, visible content within the page.
- Page margins around 10-12 mm for HTML/PDF layouts.
- Body font around 9.8-10.5 pt, line-height around 1.45-1.55.
- Section titles around 10.5-11.5 pt.
- Name around 22-26 pt.
- Avoid negative letter spacing and viewport-scaled type.

Use a dense but calm page. The page should look full, not packed.

## Top Third Rules

The top third must sell the target fit quickly.

Keep:

- Name, target role, contact.
- Current title or education status if relevant.
- 3-4 short evidence cards with strong fit signals.

Remove or move down:

- Generic keyword chips.
- "Interview expansion" or coaching notes.
- Attachment/proof reminders.
- Weak self-evaluation such as "hardworking" unless tied to evidence.
- Irrelevant certificates that do not support the target role.

## Content Selection

Prefer job-relevant evidence over decorative content:

- Education and relevant coursework for early-career candidates.
- Projects framed as transferable habits: inspection, monitoring, fault handling, documentation, safety, teamwork.
- Awards and certificates as support, not the main argument.
- Volunteer work only when it proves site discipline, process obedience, pressure handling, or communication.

Frame adjacent technical work as transferable. For example, monitoring a system can support "state inspection, anomaly detection, record keeping, follow-up handling"; do not overstate it as direct job experience.

## Photo Handling

When the user asks to add a headshot:

- Put it in the left column or header side, not as a large decorative hero.
- Use a passport-like size, roughly 25-30 mm wide and 32-38 mm tall.
- Crop with `object-fit: cover` or equivalent.
- Embed the image into final HTML/PDF/DOCX when possible so exports do not depend on temporary paths.
- Check that the photo does not push important sections off the page.

## Two-Column Balance

For two-column printable resumes:

- Put compact identity/education/course/certification material in the left column.
- Put the strongest role-fit argument, role capabilities, and projects in the wider right column.
- Move sections between columns to balance height; do not add filler just to equalize.
- If a photo is added to the left column, move only enough text to keep the left/right bottoms close.
- Prefer putting long award names in the wider column if the narrow column becomes too tall.

Aim for left and right column bottoms to be visually close. For a 794 x 1123 px A4 preview, a difference under about 20 px is usually acceptable.

## Visual Density

Avoid these failure modes:

- Large blank bands at the bottom.
- Content clipped at the bottom.
- One column ending far above the other.
- Keyword/tag blocks that make the page look crowded but add little evidence.
- Small text inside cramped cards.
- Repeated information in both columns.

To fill a page, first rebalance content and tune spacing. Only then adjust font size or card height. Do not add meaningless sections.

## Print QA

Before calling a print resume final:

- Generate a preview image or open the PDF visually.
- Confirm the PDF is one page if one page was requested.
- Confirm no content is clipped at the bottom.
- Confirm photo renders if included.
- Confirm DOCX is a valid zip with `word/document.xml`; if photos are included, confirm `word/media/` contains image files.
- Confirm private source files, contact details, photos, and screenshots are not added to public skill repositories.
