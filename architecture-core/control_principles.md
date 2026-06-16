# 控制哲学

本项目定义统一的设计哲学，用于指导所有控制机制（Control Layer）和原型（Prototype）的设计。

| 原则 | 描述 | 应用 |
|:---|:---|:---|
| **默认不可覆盖** | 数据一旦生成，默认不可修改 | 原始数据、已放行报告不可修改 |
| **状态切换显式化** | 状态变更必须记录原因与授权 | 所有状态变更需记录原因与授权人 |
| **行为可追踪** | 所有关键操作必须产生审计记录 | 产生审计事件（AuditEvent） |
| **放行前冻结** | 最终放行前必须锁定 | 报告批准后锁定，不可再编辑 |
| **异常升级** | 异常情况必须触发升级流程 | 偏差、OOS等必须触发CAPA流程 |

**原则**：所有原型设计、控制机制、SOP建议必须检查是否违反上述原则。如因现实约束必须妥协，需在相应文档中显式记录（作为"反模式"或"已知约束"）。


# Control Principles

This project defines a unified design philosophy to guide the design of all control mechanisms and prototypes.

| Principle | Description | Application |
|:---|:---|:---|
| **Immutable First** | Data, once generated, is immutable by default | Raw data, released reports cannot be modified |
| **Explicit Transition** | State changes must be explicit | All state changes require reason and authorization |
| **Traceable Action** | All critical operations must generate audit logs | Generates audit events (AuditEvent) |
| **Freeze Before Release** | Data must be frozen before final release | Report is locked after approval |
| **Exception Escalation** | Exceptions must trigger escalation | Deviations, OOS must trigger CAPA process |

**Principle**: All prototype designs, control mechanisms, and SOP recommendations must be checked against the above principles. If compromises are necessary due to real-world constraints, they must be explicitly documented (as "anti-patterns" or "known constraints").
