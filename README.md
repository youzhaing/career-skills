# Career Skills

求职场景下的 [Cursor](https://cursor.com) 项目级 Skills，可直接克隆或下载后在 Cursor 里使用，用于写简历、转 HTML、对 JD 做定制等。

## 这是什么

本仓库是一组 **Cursor Skills**：用 Markdown 写成的「说明书」，让 Cursor 里的 AI 按固定规则帮你完成求职相关任务。  
打开本仓库作为 Cursor 项目后，Agent 会自动读取 `.cursor/skills/` 下的技能，在合适时机调用。

**适合谁**：用 Cursor 写/改简历、准备求职材料的数据分析/商业分析方向同学。

## 当前包含的 Skills

| Skill | 作用 |
|-------|------|
| **data-analyst-resume-writer** | 撰写、改写、优化数据分析岗简历；支持中英文、JD 定制、项目经历润色、四字总结格式 |
| **resume-html-converter** | 把 Markdown/纯文简历转成可打印、可导出 PDF 的 HTML，A4 友好 |

### data-analyst-resume-writer

- 整份简历撰写、单段经历改写、按 JD 定制
- 项目 bullet 用「四字总结：具体说明」格式
- 中英文输出、不编造数据、强调 SQL/Python/BI/实验/指标

### resume-html-converter

- Markdown / 纯文 / 结构化笔记 → 单文件 HTML
- 内嵌 CSS、A4 打印样式、工作经历与项目层级清晰
- 可与 data-analyst-resume-writer 搭配：先写好内容，再转 HTML 导出

## 怎么用

1. **克隆或下载本仓库**到本地。
2. 用 **Cursor** 打开该文件夹（File → Open Folder）。
3. 在聊天里直接说需求，例如：
   - 「帮我按这个 JD 改一版数据分析简历」
   - 「把这段项目经历改成四字总结格式」
   - 「把这份 Markdown 简历转成可打印的 HTML」

无需额外配置，Cursor 会按描述自动选用对应 Skill。

## 仓库结构

```text
career-skills/
├── README.md
└── .cursor/
    └── skills/
        ├── data-analyst-resume-writer/   # 简历撰写与改写
        │   ├── SKILL.md
        │   ├── templates.md
        │   └── printable-resume-template.html
        └── resume-html-converter/        # 简历转 HTML
            ├── SKILL.md
            └── examples.md
```

## 扩展建议

本仓库只放**求职相关**的 Skills，例如后续可增加：

- JD 匹配与关键词提炼
- 自我介绍 / 一句话总结
- 面试故事与 STAR 整理

不建议放入与求职无关的通用分析、报表、SQL 等 Skill，以保持主题清晰、方便分享。
