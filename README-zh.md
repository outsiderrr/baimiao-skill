# baimiao-skill · 白描风格 skill

中文**白描**写作风格的 AI 文本生成约束 skill。白描通过精确呈现可感知事实、收回命名 / 评价权，将判断权留给读者。

> English version: [README.md](README.md)

## 这是什么

`SKILL.md` 是一份符合 [Claude Code](https://docs.claude.com/en/docs/claude-code)、[Claude Agent SDK](https://docs.claude.com/en/api/agent-sdk) 和 Claude.ai 格式的 Markdown skill 文件，把白描的本质定义、构成要件、实现机制、边界条件、自检流程编码为一组可调用的 AI 文本生成约束。

本 skill **只管语言风格**——不假设具体应用场景（小说 / 剧本 / RPG 对话 / 新闻特写等都可调用）。CRPG dialogue graph 节点级用法见配套仓库 [baimiao-rpg-node-skill](https://github.com/outsiderrr/baimiao-rpg-node-skill)。

## 如何使用

**Claude Code**：把 `SKILL.md` 放进项目的 `.claude/skills/baimiao/`，生成文本时调用。

**Claude Agent SDK 或 API**：把 `SKILL.md` 内容作为 system prompt 前缀注入。

**Claude.ai**：把内容贴到 project 的系统提示词里，或作为 project 文件上传。

## 内容总览

1. **本质定义** —— 4 关键词：低介入 / 事实 / 收回命名权 / 判断权留给读者
2. **5 构成要件** —— 可感知性优先 / 物理性形容词 / 物象比喻 / 无段尾点题 / 因果链非显式
3. **5 实现机制**（W-B.1–5）—— 差值 / 物质化 / 第三方折射 / 关键词位 / 动作链累积
4. **3 运作机制**（设计原理）—— 命名耗散 / 信息密度反向定律 / 前置认知依赖
5. **4 边界条件** —— 何时不用 / 慎用白描
6. **5 相邻概念辨析** —— 白描 ≠ 简洁 / 客观 / 极简主义 / 不抒情 / show-don't-tell
7. **7 条写后自检**

## 关于语言

skill 内容本身是中文写的（白描是中文美学概念，主要参考鲁迅、汪曾祺等的中文范本）。但 skill 描述的白描原则可以转用于生成任何语言的文本。

本 README 默认英文，中文版即此文件。

## License

[CC BY 4.0](LICENSE)

允许任何用途（含商业）的分享与改编。要求署名——请通过链接署名本仓库。
