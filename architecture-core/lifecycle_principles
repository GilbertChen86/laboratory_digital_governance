# Lifecycle Principles | 生命周期原则

任何核心实体（Entity）的生命周期管理，必须遵循以下统一原则：

## 1. 状态驱动 (State-Driven)
- 每个关键实体必须具有明确的状态（State）。
- 状态必须可枚举、可记录。

## 2. 显式转换 (Explicit Transition)
- 状态之间的切换必须是显式的、有记录的。
- 每次转换必须记录：时间、操作者、原因。

## 3. 责任主体 (Accountability)
- 每个状态和状态转换必须有明确的责任主体（User/Role）。

## 4. 时间戳 (Timestamping)
- 所有关键事件（创建、修改、转换、归档）必须带有准确的时间戳。

## 5. 审计性 (Auditability)
- 所有状态变化必须产生可追溯的审计事件（AuditEvent）。

## 6. 归档与保留 (Archival & Retention)
- 每个实体必须定义其归档条件和保留期限。

**适用对象**：
- Sample, Report, RawData, Instrument, CAPA, AuditEvent
