---
name: resume-html-converter
description: Convert resume content into printable HTML for browser preview and PDF export. Use when the user asks to turn a resume, CV, markdown resume, bullet points, or structured work experience into HTML, web format, printable layout, or PDF-ready output.
---

# Resume HTML Converter

## When To Use

Use this skill when the user wants to:

- Convert a resume into HTML
- Turn markdown or plain-text resume content into a browser-renderable page
- Generate a printable HTML resume for PDF export
- Reformat structured work experience into a fixed HTML layout
- Preview resume content before exporting to PDF

## Accepted Input

The source content can be any of these:

- Full resume in markdown
- Plain text resume sections
- Structured notes for work experience and projects
- A partially completed HTML template that needs content injected

## Default Output Contract

Unless the user asks otherwise, output:

1. One complete HTML document
2. Embedded CSS in the same file
3. A4-friendly print layout
4. Clear section structure
5. Work Experience with nested projects when applicable
6. Project bullets in `四字总结：内容` format when Chinese content is used

## Conversion Workflow

1. Identify the source format:
   - Markdown resume
   - Plain text
   - Structured experience notes
   - Existing HTML

2. Normalize the content into this structure:
   - Header
   - Summary
   - Skills
   - Work Experience
   - Education
   - Optional extra sections

3. When one role contains multiple projects, convert it into:
   - Company and title block
   - Project title and project date rows
   - Project bullets

4. Keep the HTML printable:
   - Avoid large margins
   - Avoid heavy colors
   - Keep font sizes compact
   - Prevent awkward page breaks inside project blocks

5. If information is missing, preserve placeholders rather than inventing details

## Formatting Rules

### Work Experience

Use this hierarchy:

1. Company / title / date
2. City or team subtitle if available
3. Multiple projects under the same job
4. Bullet rows under each project

### Bullet Layout

For Chinese resumes, prefer:

`四字总结：说明文本`

For HTML rendering, place the tag and the text in separate inline blocks or columns so wrapped lines stay aligned.

### HTML Rules

- Output semantic HTML when possible
- Keep CSS inside `<style>` unless the user explicitly wants split files
- Use print rules with `@page`
- Use `break-inside: avoid` for important resume blocks
- Reuse the visual structure from [../data-analyst-resume-writer/printable-resume-template.html](../data-analyst-resume-writer/printable-resume-template.html)

## Final Check

Before returning HTML, verify:

- The HTML is complete and directly savable as `.html`
- The layout is readable in a browser
- The structure matches the user's resume hierarchy
- Wrapped bullet text remains aligned
- No details were fabricated

## Additional Resources

- For concrete examples, read [examples.md](examples.md)
- For the printable reference layout, read [../data-analyst-resume-writer/printable-resume-template.html](../data-analyst-resume-writer/printable-resume-template.html)
