# WeChat Writing Style Skill for Claude Code
# 微信公众号写作风格 · Claude Code Skill

A Claude Code skill that guides Claude to write Chinese articles in a style optimized for WeChat Official Accounts, targeting mainland China readers.

一个 Claude Code skill，让 Claude 按照微信公众号的写作风格撰写中文文章，面向中国大陆读者。

---

## What it does / 功能介绍

This skill encodes a complete writing style guide for WeChat Official Account articles, covering:

- **结论先行**：开头直接给出核心结论，前 3 句话让读者知道文章讲什么
- **口语化高密度**：第一人称、短句、口语表达，但每段有实质信息
- **短段落留白**：每段 1–3 句，单句成段用于强调
- **具体举例**：真实工具名、真实场景、真实数据
- **格式规范**：中英文之间加空格、禁用破折号、Markdown 输出、emoji 克制
- **敏感性审查**：自动规避不适合大陆平台传播的内容
- **写作工作流**：起稿 → 敏感审查 → 事实核查 → 传播优化 → 生成备选标题

Topics covered / 常见主题：海外银行开户、跨境支付工具、AI 工具评测、NAS 自托管、投资配置框架、独立开发者出海工具链。

---

## Installation / 安装

### Option 1: Install the `.skill` file

Download `wechat-writing-style.skill` and install it via Claude Code:

```bash
claude skill install wechat-writing-style.skill
```

### Option 2: Copy `SKILL.md` manually

Place `SKILL.md` into your Claude Code skills directory:

```
~/.claude/skills/wechat-writing-style/SKILL.md
```

---

## Usage / 使用方法

Once installed, trigger the skill in Claude Code:

```
/wechat-writing-style 帮我写一篇关于 Wise 转账的公众号文章
```

Or simply mention it in your prompt:

```
按我的写作风格，写一篇介绍 Charles Schwab 海外开户的文章
```

The skill activates automatically when you ask Claude to write WeChat articles, polish content in a specific style, or mention "按我的风格写".

---

## Output format / 输出格式

Every article is delivered as a Markdown document, including:

- 正文（符合风格规范）
- 文末互动引导语
- 标准免责声明
- 5–10 个备选标题（含推荐项及推荐理由）

---

## License / 许可证

MIT License. See [LICENSE](LICENSE) for details.

---

## Author / 作者

[@yaoleifly](https://github.com/yaoleifly)
