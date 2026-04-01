✅ Claude Code 完整 Roadmap 指南：使用 · 学习 · 重建（2026 年 4 月迭代版）
所有资源均来自 2026-03-31 npm sourcemap 泄露事件后的顶级分析项目（v2.1.88，约 1900 文件 / 51.2 万行 TypeScript）。按使用 → 学习 → 重建三个维度划分 6 个阶段，每阶段标注推荐优先级。
Roadmap:
[图片]
s0:背景 S1：使用入门 S2：架构  S3： 哲学 特性 S4： 逆向 源码   S5： 重建  S6：扩展优化
 阶段 0：背景了解（30–60 分钟）
目标：搞清楚「Claude Code 到底是什么」和泄露事件全貌。
- 必读：
  - nblintao/awesome-claude-code-postleak-insights
    链接：https://github.com/nblintao/awesome-claude-code-postleak-insights
    （最佳入口 curated list，高信号索引）
  - sanbuphy/claude-code-source-code
    链接：https://github.com/sanbuphy/claude-code-source-code
    （docs/ 多语种背景报告）
  - https://learn.shareai.run/en/  
  学习CC from 网页
收获：理解 System Prompt 模块化、Agent OS 本质等核心概念。
 阶段 1：使用入门（2–4 小时）
目标：快速上手 Claude Code CLI，掌握日常工作流。
- 推荐仓库：
  1. luongnv89/claude-howto
     链接：https://github.com/luongnv89/claude-howto
     （视觉化模板 + slash commands + 10 模块教程）
  2. Cranot/claude-code-guide
     链接：https://github.com/Cranot/claude-code-guide
     （CLI 架构手册 + 15 个关键 pattern）
  3. FlorianBruniaux/claude-code-ultimate-guide
     链接：https://github.com/FlorianBruniaux/claude-code-ultimate-guide
     （cheatsheet + production-ready 模板）

收获：能独立完成简单项目。

 阶段 2：深度学习架构（6–10 小时）
目标：看懂整体架构、Prompt 组装、Agent 调度链。

- 推荐仓库：
  1. tvytlx/claude-code-deep-dive
     链接：https://github.com/tvytlx/claude-code-deep-dive
     （中文 PDF，最完整系统提示词 + Agent 调度全链路分析）
  2. 6551Team/claude-code-design-guide
     链接：https://github.com/6551Team/claude-code-design-guide
     （9-part 书式设计哲学，Unix → REPL → Agent 演进）
  3. sanbuphy/claude-code-source-code
     链接：https://github.com/sanbuphy/claude-code-source-code
     （隐私/遥测/108 个 feature gate）
  4. ComeOnOliver/claude-code-analysis
     链接：https://github.com/ComeOnOliver/claude-code-analysis
     （源码树 + 41 个工具分类 + 模块边界）

收获：明白 Claude Code 是一个完整的 Agent Operating System。

 阶段 3：高级特性 & 设计哲学（8–12 小时）
目标：掌握隐藏机制、roadmap、哲学 trade-off。

- 推荐仓库：
  1. FlorianBruniaux/claude-code-ultimate-guide
     链接：https://github.com/FlorianBruniaux/claude-code-ultimate-guide
     （41 个 Mermaid 图 + 219 个模板 + 271 道 quiz，最强教学书）
  2. paullarionov/claude-certified-architect
     链接：https://github.com/paullarionov/claude-certified-architect
     （PART I 理论基础 + 练习题）
  3. 6551Team/claude-code-design-guide
     链接：https://github.com/6551Team/claude-code-design-guide
     （上下文工程 4 层模型、多 Agent 协调器）
  4. sanbuphy/claude-code-source-code
     链接：https://github.com/sanbuphy/claude-code-source-code
     （KAIROS、Undercover Mode、killswitch）

收获：学会用「设计哲学」视角评估 Agent 工具。



 阶段 4：逆向工程 & 源码拆解（10–15 小时，选做）
目标：真正读懂 1900 个文件是怎么组织的。

- 推荐仓库：
  1. LeonTang-LeonTang/CLAUDE-CODE-XRAY
     链接：https://github.com/LeonTang-LeonTang/CLAUDE-CODE-XRAY
     （5 层架构 + 执行流 + Mermaid 可视化 + 重构指南）
  2. ComeOnOliver/claude-code-analysis
     链接：https://github.com/ComeOnOliver/claude-code-analysis
     （37 个子目录详解 + 状态机）
  3. amitshekhariitbhu/claude-code-codebase-architecture-report
     链接：https://github.com/amitshekhariitbhu/claude-code-codebase-architecture-report
     （生产级技术栈决策）
  4. asgeirtj/system_prompts_leaks
     链接：https://github.com/asgeirtj/system_prompts_leaks
     （全量 Prompt 提取 + 版本历史）

收获：掌握 Query Engine、Context Builder 等底层设计模式。



 阶段 5：重建实践（Clean-room 重构，12–20 小时，进阶核心）
目标：自己动手复现甚至改进 Claude Code。

- 推荐仓库（按难度递增）：
  1. shareAI-lab/learn-claude-code
     链接：https://github.com/shareAI-lab/learn-claude-code
     （12 阶段课程 + Python/Bash nano 重构，最推荐动手党）
  2. Kuberwastaken/claude-code
     链接：https://github.com/Kuberwastaken/claude-code
     （Rust 版 clean-room 重实现 + 行为规格 spec/ + 改进并发）
  3. chauncygu/collection-claude-code-source-code
     链接：https://github.com/chauncygu/collection-claude-code-source-code
     （TS 原味存档 + Python 简化版对比）
  4. FlorianBruniaux/claude-code-ultimate-guide
     链接：https://github.com/FlorianBruniaux/claude-code-ultimate-guide
     （模板 + 威胁模型，可直接用于重建）

收获：理解「模型是 Agent，代码是 Harness」的本质。



 阶段 6：生产扩展 & 优化（持续进阶）
目标：把 Claude Code 变成生产级工具。

- 推荐仓库：
  1. affaan-m/everything-claude-code
     链接：https://github.com/affaan-m/everything-claude-code
     （Skills/Instincts/Memory/安全扫描 + 扩展）
  2. FlorianBruniaux/claude-code-ultimate-guide
     链接：https://github.com/FlorianBruniaux/claude-code-ultimate-guide
     （security-hardening + MCP 生态）

收获：掌握性能优化、插件生态、威胁防御。



 完整资源总表（按角度分类，已附链接）

| 类型               | 仓库链接                                      | 核心价值                              | 推荐指数 |
| Curated List      | nblintao/awesome-claude-code-postleak-insights | 高信号索引入口  | ★★★★★   |
| 中文 PDF 深度报告 | tvytlx/claude-code-deep-dive | Prompt + Agent 全链路              | ★★★★★   |
| 多语言分析        | sanbuphy/claude-code-source-code | 隐私/roadmap/隐藏特性        | ★★★★★   |
| 设计哲学书        | 6551Team/claude-code-design-guide | 为什么这样设计                  | ★★★★★   |
| 终极教学指南      | FlorianBruniaux/claude-code-ultimate-guide | 模板+quiz+41 图，最全面教学| ★★★★★   |
| 动手重构课程      | shareAI-lab/learn-claude-code | 12 阶段 Python nano 重建              | ★★★★★   |
| 逆向可视化        | LeonTang-LeonTang/CLAUDE-CODE-XRAY | 执行流 + 重构指南         | ★★★★☆   |
| 模块级拆解        | ComeOnOliver/claude-code-analysis | 源码树 + 工具分类                 | ★★★★☆   |
| Rust Clean-room   | Kuberwastaken/claude-code | 生产级 Rust 重实现                        | ★★★★☆   |
| 生产优化          | affaan-m/everything-claude-code | Skills + 安全 + 扩展                  | ★★★★☆   |

补充资源（链接已确认）：
- asgeirtj/system_prompts_leaks：https://github.com/asgeirtj/system_prompts_leaks （Prompt 专项）
- paullarionov/claude-certified-architect：https://github.com/paullarionov/claude-certified-architect （认证式理论）

学习建议：推荐顺序 0 → 1 → 2 → 3 → 5 → 6。总计 3–4 周可走完闭环。先 star 最强教学仓库（FlorianBruniaux + shareAI-lab）开始冲！
答案变得廉价，思考和问题开始闪光，以上仓库附带噪音，还请自辩
