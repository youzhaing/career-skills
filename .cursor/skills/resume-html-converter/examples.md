# Examples

## Example 1: Markdown Resume To HTML

Input:

```markdown
# 张三

## 个人简介
3 年数据分析经验，熟悉 SQL、Python、Tableau。

## 工作经历
### A 公司 | 数据分析师
2022.06 - 至今 | 上海

#### 用户增长分析项目
2024.01 - 2024.09
- 指标搭建：定义转化漏斗指标并搭建监控报表
- 问题诊断：分析核心环节流失原因并输出优化建议
```

Expected output shape:

- One full HTML document
- Header, summary, skills, work experience, education sections
- Nested project block inside work experience
- Bullet tag and text separated for aligned wrapping

## Example 2: Structured Notes To HTML

Input:

```text
姓名：李四
岗位：数据分析师
公司：某电商平台
任职时间：2021.07-2024.12
项目1：经营分析体系建设，2024.01-2024.08
项目点：
经营复盘：搭建周度经营分析框架
流程优化：优化自动化报表流程
```

Expected conversion:

1. Turn the notes into semantic sections
2. Map company and role to one experience block
3. Map project1 into a nested project block
4. Preserve the bullet label format

## Example 3: Preview-Friendly HTML

If the user asks for HTML preview or printable PDF:

- Return a self-contained HTML file
- Use embedded CSS
- Use A4 page settings
- Keep margins and spacing compact
- Ensure the output can be opened directly in a browser
