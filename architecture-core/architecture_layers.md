# Architecture Layers | 架构分层

本项目所有内容（文章、模型、原型）必须归属于以下某个固定层次。

| Layer | Purpose | Example Output |
|:---|:---|:---|
| **Observation** | 现实观察 | 从业者经验、访谈、现场问题 |
| **Model** | 抽象规律 | 冲突模型、形式化模型 |
| **Lifecycle** | 生命周期定义 | Sample Lifecycle, CAPA Lifecycle |
| **State Machine** | 状态转换控制 | Report State Machine |
| **Data Structure** | 数据结构定义 | Event Log Schema |
| **Control Layer** | 控制机制设计 | Mandatory Review Control |
| **Prototype** | 最小实现 | audit-log-lite, deviation-tracker |

**处理流程**：
1. 新主题进入 → 确定核心 Entity
2. 按上述层次逐一推进
3. 每个层次产出物必须放入对应目录
4. 例如：Audit Trail 不再是独立主题，而是 AuditEvent 实体的 Control Layer 设计。
