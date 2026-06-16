# 架构分层

本项目所有内容（文章、模型、原型）必须归属于以下某个固定层次。

| 层次 | 目的 | 产出示例 |
|:---|:---|:---|
| **观察层** | 现实观察 | 从业者经验、访谈、现场问题 |
| **模型层** | 抽象规律 | 冲突模型、形式化模型 |
| **生命周期层** | 生命周期定义 | 样品生命周期、CAPA生命周期 |
| **状态机层** | 状态转换控制 | 报告状态机 |
| **数据结构层** | 数据结构定义 | 事件日志结构 |
| **控制层** | 控制机制设计 | 强制审核控制 |
| **原型层** | 最小实现 | 轻量审计日志、偏差追踪器 |

**处理流程**：新主题进入 → 确定核心实体 → 按上述层次逐一推进 → 每个层次产出物放入对应目录。

**示例**：审计追踪不再是独立主题，而是 AuditEvent 实体的控制层设计。


# Architecture Layers

All content (articles, models, prototypes) in this project must belong to one of the following fixed layers.

| Layer | Purpose | Example Output |
|:---|:---|:---|
| **Observation** | Real-world observation | Practitioner experience, interviews, field issues |
| **Model** | Abstract patterns | Conflict models, formalization models |
| **Lifecycle** | Lifecycle definition | Sample Lifecycle, CAPA Lifecycle |
| **State Machine** | State transition control | Report State Machine |
| **Data Structure** | Data structure definition | Event Log Schema |
| **Control Layer** | Control mechanism design | Mandatory Review Control |
| **Prototype** | Minimal implementation | audit-log-lite, deviation-tracker |

**Processing Workflow**: New topic enters → Identify core Entity → Advance layer by layer as per above → Place each layer's output into corresponding directory.

**Example**: Audit Trail is no longer an independent topic, but a Control Layer design for the AuditEvent Entity.
