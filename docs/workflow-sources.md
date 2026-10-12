# 工作流来源

本站 `AGENTS.md` 的方法论来自下面两个开源项目，取其精华、按中文习惯重写为精简版。

## affaan-m/ECC

https://github.com/affaan-m/ECC

Agent harness 性能优化体系：Skills、直觉（instincts）、记忆、安全、research-first 开发，面向 Claude Code / Codex / Opencode / Cursor。

取用了：
- **Skills 优先**：可复用的工作流沉淀为 skill，而不是一次性 prompt。
- **Hooks**：触发式自动化（格式化、lint、提醒），只挂在工具调用与生命周期事件上。
- **Subagents**：主 agent 委派限定范围的子任务，规划 / 评审 / 测试各司其职。
- **Rules 目录**：按关注点拆分的常驻规则（安全、代码风格、测试、git 工作流）。
- **上下文窗口管理**：MCP / 插件按需启用，保持工具数量精简。

## multica-ai/andrej-karpathy-skills

https://github.com/multica-ai/andrej-karpathy-skills

单个 `CLAUDE.md`，源自 Andrej Karpathy 对 LLM 写代码常见坑的观察。

取用了四条铁律：
1. **Think Before Coding** — 先想再写，不确定就问。
2. **Simplicity First** — 简单优先，不做没被要求的东西。
3. **Surgical Changes** — 手术刀式修改，只碰必须碰的。
4. **Goal-Driven Execution** — 目标驱动，把任务翻译成可验证的目标。
