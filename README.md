# wechat-writing-style

**A reusable Chinese editorial writing system for WeChat Official Account content.**  
**一个面向微信公众号内容创作的可复用中文编辑写作系统。**

`wechat-writing-style` packages a specific writing taste into a practical skill: clear conclusions, dense information, conversational rhythm, and distribution-aware structure.  
`wechat-writing-style` 想做的不是“写一篇像样的文章”，而是把一种清晰、有传播力、适合大陆平台的写作判断，沉淀成可以反复调用的系统。

It is designed for writers, operators, and AI-assisted content workflows that need:
它适合那些希望把写作流程产品化的人，尤其是：

- faster first drafts without losing voice  
  提高起稿速度，同时不丢掉个人风格
- stronger structure for public-account reading habits  
  更适合公众号阅读习惯的结构设计
- distribution-aware wording for mainland China audiences  
  更适合中国大陆传播环境的表达方式
- repeatable editorial quality across topics  
  在不同主题下保持稳定的编辑质量

## Why this exists / 为什么做它

Good writing is often treated as intuition. I’m more interested in what happens when taste, rhythm, and editorial judgment become reusable infrastructure.  
很多人把好写作理解成“天赋”或“手感”，我更关心的是：当审美、节奏和编辑判断力被系统化之后，会不会变成一种可复用基础设施。

That is the core idea behind this project.  
这就是这个项目背后的核心判断。

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
