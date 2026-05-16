# The Unified Guide to AI Best Practices

> A unified guide on how to use AI well, distilled from all official documentation by OpenAI and Anthropic.

[中文版 / Chinese version](./README.cn.md)

This project integrates every core article on the topic of "how to use AI well" published by OpenAI and Anthropic across their official websites — organized by underlying principles rather than by company — into a single, systematic best-practices guide.

📖 **[Read the full guide →](./AI-Best-Practices-Unified-Guide/AI_最佳实践_统一指南.md)** *(currently in Chinese; English translation in progress)*

---

## Why this project exists

The internet is flooded with "how to use AI" content. Most of it is recycled prompt templates or one-off tips from individual bloggers.

Meanwhile, the actual source — OpenAI and Anthropic themselves — has published an enormous amount of high-signal documentation explaining how their models should be used, why they were designed this way, and which parameters fit which scenarios. But this material is scattered across both companies' docs sites, engineering blogs, cookbooks, and white papers. Nobody has put it together.

This project does three things:

1. **Reads every relevant official document from both companies** — guides, best practices, engineering blogs, white papers, cookbooks. All of it.
2. **Organizes by underlying principle, not by company** — surfacing the cross-cutting truths instead of just listing items.
3. **Preserves the disagreements between the two companies** — often the most informative part: it tells you which practices are universal truths versus model-specific quirks.

The result is a ~30,000-word integrated guide.

---

## What's inside

| # | Chapter | Content |
|---|---------|---------|
| 1 | Foundational Principles | The model can't read your mind / Treat it like a "smart new colleague" / Prompt engineering is iterative |
| 2 | Universal Prompting Techniques | Clear instructions, context, examples, XML structuring, roles, long context, output format, instruction hierarchy |
| 3 | Letting the Model "Think" | Reasoning models vs. GPT models, effort parameters, when to invoke thinking |
| 4 | Tools & Agent Construction | When to use agents, workflow vs. agent, five core patterns, tool design, parallel calls, controlling eagerness |
| 5 | Context Engineering | Context rot, multi-window workflows, Skills and progressive disclosure, state management |
| 6 | Safety & Guardrails | Layered defense, seven guardrail types, human-in-the-loop, prompt injection defense |
| 7 | Testing & Evaluation | Success criteria, LLM-as-judge, systematic changes |
| 8 | Coding Practices | CLAUDE.md / AGENTS.md, avoiding test-hacking, avoiding over-engineering, frontend design |
| 9 | Common Pitfalls & Anti-Patterns | The 9 most common traps |
| 10 | Where the Two Companies Diverge | 5 explicit differences |
| 11 | 9 Production-Grade Prompt Templates | Ready to copy-paste |
| 12 | Conclusion: Six Layered Capabilities | Reducing hundreds of pages to a set of essential principles |

---

## Who this is for

- **Heavy AI users** — anyone working daily with ChatGPT / Claude who wants to systematize their scattered intuitions
- **Developers / prompt engineers** — building AI products, calling APIs, constructing agents
- **Product / operations / management** — knowledge workers who need to understand what AI can do, where its limits are, and how to deploy it
- **Researchers / learners** — anyone who wants to build a mental model of AI usage from primary sources

---

## Sources

### OpenAI
- *A Practical Guide to Building Agents* (official business white paper)
- *Prompt engineering* (OpenAI API docs)
- *GPT-5 prompting guide* (OpenAI Cookbook)
- *GPT-5.1 prompting guide*
- *Prompt guidance* (GPT-5.4 / 5.5)
- *Reasoning best practices*
- *Prompt engineering best practices for ChatGPT* (Help Center)
- OpenAI Academy prompt engineering resources

### Anthropic
- *Prompting best practices* (Claude API docs)
- *Prompt engineering overview*
- *Building effective agents* (engineering blog)
- *Building agents with the Claude Agent SDK*
- *Claude Code best practices*
- *Writing effective tools for agents*
- *Effective harnesses for long-running agents*
- *Equipping agents for the real world with Agent Skills*
- *Define success criteria and build evaluations*

---

## How to read it

**First pass**: Read chapters 1 through 12 in order to build the overall mental map.

**As a reference book**: Jump to specific chapters when problems come up —
- Don't know how to write a prompt → Chapter 2
- Wondering whether your agent project needs a framework → Chapter 4
- Prompt changes are making things worse → Chapters 7, 9
- AI keeps over-engineering your code → Chapter 8
- Just want templates to copy → Chapter 11

**Import into your note-taking tool**: The document is in Markdown and can be loaded directly into Notion, Obsidian, Logseq, or any other tool to become part of your personal knowledge base.

---

## Contributing

PRs and issues are welcome:

- New documents published by either company that should be integrated
- Corrections, additions, or better translations of existing content
- Counter-examples or supplemental experience from the field
- New prompt templates or production practices
- Comparable content from other LLM vendors (Google, Mistral, etc.) for cross-reference

Models change. This guide is maintained as a living document, not a one-shot artifact.

---

## License

This project's content is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to share, adapt, and use commercially, with attribution required.

Original quoted content from official documentation remains the copyright of OpenAI and Anthropic respectively. This project only integrates, organizes, translates, and interprets it.

---

## Closing thought

> Models keep changing. Last year's "best practices" may be obsolete this year. But the underlying principles that appear over and over in the official docs — from the GPT-3 era to GPT-5, from Claude 2 to Opus 4.7 — have barely shifted.
>
> **Understanding principles is worth more than memorizing incantations.**

If you find this useful, please Star ⭐ to support the project, and share it with anyone who might benefit.
