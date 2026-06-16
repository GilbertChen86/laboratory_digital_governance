# Core Entities | 核心实体

本项目所有分析、模型、控制机制，均围绕以下唯一核心实体展开。任何新主题必须映射到至少一个实体。

| Entity | Description | Key Attributes |
|:---|:---|:---|
| **Sample** | 检测对象 | ID, Type, Matrix, Quantity, Condition |
| **Report** | 最终交付物 | ID, Template, Data, Signatories |
| **RawData** | 原始数据（含元数据） | File, Timestamp, Operator, Instrument |
| **Instrument** | 检测设备 | ID, Type, Calibration, Status |
| **User** | 系统参与者 | ID, Role, Permissions |
| **AuditEvent** | 审计追踪事件 | User, Action, Timestamp, Entity |
| **CAPA** | 纠正与预防措施 | ID, Trigger, RootCause, Action, Status |

**原则**：
- 后续所有文章、模型、数据结构、原型设计，必须引用上述实体。
- 如需引入新实体，必须在此文件更新并经架构评审。
