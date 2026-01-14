## 🚀 优化目标
解决大纲扩写正文时出现的重复、啰嗦（车轱辘话）问题，从简单的“扩写”转向“演绎”。

## 🛠 待实现 Skills (Agentic Workflow)

### 1. 核心功能开发
- [ ] **Skill A: Beat_Sheet_Generator (节拍细化器)**
    - [ ] 编写 Prompt：将一句话大纲拆解为 5-10 个物理动作/节拍。
    - [ ] 逻辑实现：作为正文生成的前置步骤。
- [ ] **Skill B: Context_Slicer (上下文切片器)**
    - [ ] 实现滑动窗口：只保留最近 500-800 字 context。
    - [ ] 实现摘要提取：提取前文关键信息作为 Global Context。
    - [ ] 添加负面约束（Negative Constraint）：禁止重复已发生的描写。
- [ ] **Skill C: Narrative_Bridge (叙事桥接器)**
    - [ ] 检测场景跳跃，自动生成过渡段（如“十分钟后”）。
- [ ] **Skill D: Text_Critic (自我审查器)**
    - [ ] 编写 Prompt：检查重复语句，删除冗余。

### 2. Prompt 调优
- [ ] 增加指令：`Do not end the scene with a summary` (禁止总结结尾)。
- [ ] 增加指令：`Use active verbs` (强制动词优先)。

### 3. 参数配置 (Configuration)
- [ ] 调整 Temperature 至 0.8 - 1.0。
- [ ] 设置 Frequency Penalty 至 0.3 - 0.6 (核心防重复参数)。
