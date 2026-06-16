# Control Principles | 控制规则

本项目定义统一的设计哲学，用于指导所有控制机制（Control Layer）和原型（Prototype）的设计。

| Principle | Description | Application |
|:---|:---|:---|
| **Immutable First** | 默认不可覆盖 | 原始数据、已放行报告不可修改 |
| **Explicit Transition** | 状态切换必须显式 | 所有状态变更需记录原因与授权 |
| **Traceable Action** | 所有关键行为可追踪 | 产生审计事件（AuditEvent） |
| **Freeze Before Release** | 放行前冻结 | 报告批准后锁定，不可再编辑 |
| **Exception Escalation** | 异常必须升级 | 偏差、OOS等必须触发CAPA流程 |

**原则**：
- 所有原型设计、控制机制、SOP建议必须检查是否违反上述原则。
- 如因现实约束必须妥协，需在相应文档中显式记录（作为“反模式”或“已知约束”）。
