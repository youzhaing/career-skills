---
name: data-analyst-resume-writer
description: Write and tailor resumes for data analysts, including bilingual resume drafting, experience rewrite, project bullet polishing, and JD alignment. Use when the user asks to write, rewrite, polish, optimize, tailor, or translate a data analyst resume, CV, bullet points, self-summary, or project experience, especially for SQL, Python, dashboard, experiment, KPI, analytics, and business impact narratives.
---

# Data Analyst Resume Writer

## When To Use

Use this skill when the user wants help with any of the following:

- Writing a full data analyst resume or CV
- Rewriting raw experience into resume bullet points
- Tailoring a resume to a job description
- Improving ATS keyword coverage
- Translating resume content between Chinese and English
- Strengthening project descriptions for SQL, Python, BI, experimentation, metrics, forecasting, or analytics work
- Generating HTML resumes for printing or PDF export

## Default Positioning

Assume the target profile is a data analyst with a technical and business-facing style:

- Emphasize problem framing, analysis method, tooling, and measurable impact
- Prefer precise verbs and concrete outcomes over generic claims
- Highlight SQL, Python, Excel, BI tools, experimentation, metrics systems, dashboards, and stakeholder collaboration when relevant
- Never invent numbers, scale, or outcomes

## Working Style

1. Identify the task type first:
   - Full resume
   - One section rewrite
   - JD-based tailoring
   - Personal summary
   - Project experience rewrite

2. If information is incomplete, ask only for the missing essentials:
   - Target role and level
   - Years of experience
   - Industry or business domain
   - Tools used
   - Key projects
   - Metrics influenced
   - Preferred output language

3. Convert raw experience into achievement-oriented bullets using this order:
   - Business context
   - Action taken
   - Method or tool
   - Result or metric
   - Business impact

4. Keep the writing compact:
   - 1 line for simple work
   - 2 lines max for strong project bullets
   - Avoid long narrative paragraphs inside experience sections

5. Default work-experience structure:
   - Company / title / date range
   - Multiple projects under the same work experience when applicable
   - Each project includes project title, date, and bullet points

## Rewrite Rules

### Bullet Formula

Use this default formula:

`Action + scope + method/tool + measurable result + business impact`

For project bullets, prefer this visible structure:

`四字总结：具体说明`

Example transformation:

- Raw: "做了用户分析，给运营看报表。"
- Better: "搭建用户留存与转化分析框架，使用 SQL 和 Python 输出周度监控报表，支持运营定位流失环节并优化核心转化路径。"

Examples of four-character labels:

- `指标搭建：`定义核心业务指标口径并落地监控报表
- `实验分析：`评估活动效果并输出策略建议
- `归因拆解：`分析转化波动的关键驱动因素
- `流程优化：`自动化报表流程并缩短交付时间

### Good Resume Language

Prefer:

- Built, automated, analyzed, designed, defined, monitored, optimized, identified, improved, validated
- Quantified outcomes such as accuracy, efficiency, revenue, conversion, retention, cost, SLA, adoption, time saved

Avoid:

- Responsible for
- Assisted with
- Participated in
- Familiar with
- Hard-working, team player, fast learner

### Metrics Rule

- Use real numbers only when the user provided them
- If a result should be quantified but the metric is missing, mark it clearly:
  - Chinese: `[量化结果待补充]`
  - English: `[metric needed]`

## JD Tailoring Rules

When the user provides a job description:

1. Extract required skills, domain terms, and business priorities
2. Map the user's experience to those requirements
3. Reorder bullets so the most relevant evidence appears first
4. Add missing but truthful keywords already supported by the user's background
5. Flag obvious gaps instead of hiding them

## Bilingual Output Rules

- If the user requests Chinese, write in polished Chinese resume style
- If the user requests English, use concise business English suitable for analyst roles
- If the user asks for bilingual output, keep Chinese and English meaning aligned rather than word-for-word literal translation

## Output Formats

### Full Resume

Use this section order unless the user asks otherwise:

1. Header
2. Professional Summary
3. Core Skills
4. Work Experience
5. Education
6. Optional: Certifications or Awards

Inside `Work Experience`, prefer this hierarchy when the user handled multiple initiatives in one role:

1. Company / title / date
2. Project title + project date
3. Project bullets in `四字总结：内容` format

### HTML Resume

If the user asks for HTML, printing, or PDF export:

1. Output semantic HTML with embedded CSS by default
2. Use A4-friendly spacing and print rules
3. Keep sections compact enough for PDF export and one-page resume styles when content volume allows
4. In project bullets, separate the four-character label and description so wrapped lines align cleanly
5. Follow the printable template in [printable-resume-template.html](printable-resume-template.html)

### Section Rewrite

Return in this order:

1. Revised version
2. Optional stronger alternative if the source material is weak
3. Missing information needed to improve it further

## Quality Checklist

Before finalizing, check:

- The wording is specific and not generic
- Each bullet shows action, method, and outcome where possible
- Tools are visible when they strengthen credibility
- Business impact is clear
- The text matches the target data analyst role
- No fabricated achievements were introduced

## Additional Resources

- For full resume templates and bullet templates, read [templates.md](templates.md)
- For printable HTML output, read [printable-resume-template.html](printable-resume-template.html)
