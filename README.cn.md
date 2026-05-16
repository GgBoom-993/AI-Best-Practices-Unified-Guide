# AI 最佳实践统一指南

> A unified guide on how to use AI well, distilled from all official documentation by OpenAI and Anthropic.

整合 OpenAI 与 Anthropic 两家公司官方文档中关于"如何用好 AI"主题的全部核心文章，按底层原则而非按公司分类，形成一份系统化的中文最佳实践指南。

📖 **[阅读完整指南 →](./AI-Best-Practices-Unified-Guide/AI最佳实践统一指南.pdf)**

---

## 为什么有这个项目

网上关于"AI 怎么用"的内容多到爆炸，但大部分是抄来抄去的 prompt 模板，或者博主个人琢磨出来的小窍门。

真正的源头——OpenAI 和 Anthropic 自己——其实写了大量极其干货的文档，告诉你他们的模型该怎么用、为什么这么设计、什么场景用什么参数。这些内容散落在两家的官网、文档站、工程博客、cookbook、白皮书里，没有人系统地把它们整理在一起。

这个项目做了三件事：

1. **把两家所有相关官方文档读完**——指南、最佳实践、工程博客、白皮书、cookbook，全部
2. **按底层原则而非公司来组织**——找出贯穿性的本质，而不是简单罗列
3. **保留两家的分歧点**——这部分往往最有信息量，告诉你哪些是普遍真理、哪些是特定模型的怪癖

最终输出一份约 3 万字的整合指南。

---

## 内容速览

| # | 章节 | 内容 |
|---|---|---|
| 1 | 底层原则 | 模型不会读心 / 把它当成"新同事" / 提示工程是迭代的 |
| 2 | 通用提示技术 | 清晰指令、上下文、示例、XML 结构化、角色、长上下文、格式控制、指令链 |
| 3 | 让模型"思考" | 推理模型 vs GPT 模型、effort 参数、思考触发 |
| 4 | 工具使用与 Agent 构建 | 何时该用 Agent、工作流 vs Agent、五种核心模式、工具设计、并行调用、积极性控制 |
| 5 | 上下文工程 | Context Rot、多窗口工作流、Skills 渐进式披露、状态管理 |
| 6 | 安全与护栏 | 多层防御、七类护栏、人工介入、Prompt Injection 防御 |
| 7 | 测试与评估 | 成功标准、LLM as Judge、系统性改动 |
| 8 | 编程场景特殊实践 | CLAUDE.md / AGENTS.md、避免 hack 测试、反过度工程、前端设计 |
| 9 | 常见陷阱与反模式 | 9 个最常见的坑 |
| 10 | 两家公司的分歧点 | 5 处明确差异 |
| 11 | 9 个工业级提示模板 | 可直接复用 |
| 12 | 总结：六条递进能力 | 把上百页材料浓缩为一组本质原则 |

---

## 适合谁读

- **AI 重度用户**——日常用 ChatGPT / Claude 工作的人，想把散乱经验系统化
- **开发者 / Prompt 工程师**——做 AI 产品、调 API、构建 Agent 的人
- **产品 / 运营 / 管理**——需要理解 AI 能做什么、边界在哪、怎么落地的知识工作者
- **研究 / 学习者**——希望从源头建立 AI 使用心智模型的人

---

## 资料来源

### OpenAI
- 《A Practical Guide to Building Agents》（OpenAI 官方业务白皮书）
- 《Prompt engineering》（OpenAI API 文档）
- 《GPT-5 prompting guide》（OpenAI Cookbook）
- 《GPT-5.1 prompting guide》
- 《Prompt guidance》（GPT-5.4 / 5.5 提示指南）
- 《Reasoning best practices》
- 《Prompt engineering best practices for ChatGPT》(Help Center)
- OpenAI Academy 提示工程资源

### Anthropic
- 《Prompting best practices》（Claude API 文档）
- 《Prompt engineering overview》
- 《Building effective agents》（工程博客）
- 《Building agents with the Claude Agent SDK》
- 《Claude Code best practices》
- 《Writing effective tools for agents》
- 《Effective harnesses for long-running agents》
- 《Equipping agents for the real world with Agent Skills》
- 《Define success criteria and build evaluations》

---

## 怎么读

**第一次读**：从第 1 章读到第 12 章，建立整体框架感。

**当作工具书**：遇到具体问题时按章节速查——
- 不知道怎么写 prompt → 第 2 章
- Agent 项目要不要上框架 → 第 4 章
- prompt 改完效果反而变差 → 第 7、9 章
- 用 AI 写代码总是过度工程 → 第 8 章
- 想直接拿模板用 → 第 11 章

**导入笔记工具**：本文档为 Markdown 格式，可直接导入 Notion / Obsidian / 飞书 / Logseq 等工具，建立个人知识库。

---

## 贡献

欢迎提交 PR 或 Issue：

- 两家公司的新文档发布、需要纳入整合
- 已有内容的勘误、补充、更准确的翻译
- 实战中发现的反例或补充经验
- 新的 prompt 模板或工业实践
- 来自其他 LLM 厂商（Google、Mistral 等）官方文档的对比补充

模型在变，文档也要跟着变。这是一份持续维护的指南，不是一锤子买卖。

---

## License

本项目内容采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 许可——可自由分享、修改、商用，需署名。

引用的官方文档原始内容版权归 OpenAI 和 Anthropic 所有。本项目仅对其进行整合、归纳、翻译与解读。

---

## 最后

> 模型一直在变，去年的"最佳实践"今年可能就过时了。但官方文档里反复出现的那些底层原则，从 GPT-3 时代到现在的 GPT-5、从 Claude 2 到现在的 Opus 4.7，几乎没怎么变过。
>
> **理解原则比记住咒语更值钱。**

如果这份整理对你有用，欢迎 Star ⭐ 支持，也欢迎分享给可能需要的朋友。
