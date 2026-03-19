# 外接执行层

经研龙虾不仅可以在内部完成研究规划、设计诊断、审查闭环与论文表达，也可以把**具体实施任务**外接给 Claude Code、Codex 等执行器。

## 目标

形成一种双层工作流：
- **经研龙虾负责管理、拆解、审查、交互**
- **外部执行器负责具体代码、脚本、批处理与工程实施**

这意味着经研龙虾既可以作为独立研究工作台，也可以套在更底层的执行型工作流外面。

## 当前已接入的外部能力

### 1. Claude Code
已导入：`imported-skills/claude-code`

适合：
- 批量文件生成
- 代码与脚本实现
- 结构化重构
- 本地工程级修改

### 2. Codex Orchestrator
已导入：`imported-skills/codex-orchestrator`

适合：
- 面向执行型 coding workflow 的任务分发
- 较复杂的自动化编码与迭代修改

### 3. OpenClaw PPT Generator
已导入：`imported-skills/openclaw-ppt-generator`

适合：
- 直接生成展示用 PPT
- 比赛答辩稿、简报、项目介绍材料

## 推荐协作模式

### 模式 A：龙虾主导，执行器落地
1. 经研龙虾形成研究问题 / 设计 / 数据方案
2. 经研龙虾将实现任务拆解为代码任务
3. Claude Code / Codex 执行代码与文件生成
4. 经研龙虾接回结果，做 reviewer / critic / defender / fixer 闭环

### 模式 B：龙虾主导，展示物料自动化
1. 经研龙虾先整理项目书短版或 demo 内容
2. 使用 PPT / poster 类 skill 生成展示材料
3. 再由龙虾继续打磨内容与结构

## 在经研龙虾工作流中的位置

经研龙虾不替代 Claude Code 或 Codex，而是站在它们之上：
- 负责研究逻辑
- 负责任务编排
- 负责质量审查
- 负责与用户交互
- 负责把执行结果重新拉回学术闭环
