# 核心实体

本项目所有分析、模型、控制机制，均围绕以下唯一核心实体展开。任何新主题必须映射到至少一个实体。

| 实体 | 描述 | 关键属性 |
|:---|:---|:---|
| **Sample** | 检测对象 | ID, Type, Matrix, Quantity, Condition |
| **Report** | 最终交付物 | ID, Template, Data, Signatories |
| **RawData** | 原始数据（含元数据） | File, Timestamp, Operator, Instrument |
| **Instrument** | 检测设备 | ID, Type, Calibration, Status |
| **User** | 系统参与者 | ID, Role, Permissions |
| **AuditEvent** | 审计追踪事件 | User, Action, Timestamp, Entity |
| **CAPA** | 纠正与预防措施 | ID, Trigger, RootCause, Action, Status |

**原则**：后续所有文章、模型、数据结构、原型设计，必须引用上述实体。如需引入新实体，必须在此文件更新并经架构评审。


# Core Entities

All analyses, models, and control mechanisms in this project are built around the following unique core entities. Any new topic must map to at least one entity.

| Entity | Description | Key Attributes |
|:---|:---|:---|
| **Sample** | Test object | ID, Type, Matrix, Quantity, Condition |
| **Report** | Final deliverable | ID, Template, Data, Signatories |
| **RawData** | Raw data (including metadata) | File, Timestamp, Operator, Instrument |
| **Instrument** | Test equipment | ID, Type, Calibration, Status |
| **User** | System participant | ID, Role, Permissions |
| **AuditEvent** | Audit trail event | User, Action, Timestamp, Entity |
| **CAPA** | Corrective and Preventive Action | ID, Trigger, RootCause, Action, Status |

**Principle**: All subsequent articles, models, data structures, and prototypes must reference the entities defined here. Any new entity must be updated in this file and reviewed.
