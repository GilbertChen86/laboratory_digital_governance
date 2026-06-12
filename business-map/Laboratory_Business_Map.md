# Module 1: Laboratory Business Map | 模块1：实验室业务全景图

## Layer 1: Phenomena | 现象

### 1.1 Role Overlap | 角色兼职

同一人在多个步骤中担任不同角色。常见的兼职情况：

| Role Combination | Frequency | Risk | Chinese |
|-----------------|-----------|------|---------|
| Contract Review + Report Approval | Common in small labs | No cross-validation | 合同评审+报告批准，无交叉验证 |
| Data Review + Report Approval | Common in small labs | Superficial review | 数据审核+报告批准，审核流于形式 |
| Sample Admin + Planner | Common | Acceptable | 样品管理员+分板人员，风险可接受 |

### 1.2 Data Objects by Step | 按步骤的数据对象

| Step | Data Objects | Format | Chinese |
|------|--------------|--------|---------|
| Customer Request | Test application form, Confidentiality agreement | Paper/CRM | 检测申请表、保密协议 |
| Contract Review | Commercial contract | Paper/CRM | 商业合同 |
| Sample Reception | Logistics receipt, Sample label, Storage record | LIMS/Paper | 物流单据、样品标签、入库登记 |
| Task Assignment | Storage record, Sample label, Application form, Processing record | LIMS/Paper | 出入库登记、样品标签、检测申请表、处理记录 |
| Testing Execution | Raw data record, Processing record, Environmental record, Instrument log | Paper/LIMS | 原始记录、处理记录、环境记录、仪器使用记录 |
| Data Review | Application form, Raw data record, Processing record | Paper | 检测申请表、原始记录、处理记录 |
| Report Approval | Application form, Report template, Final report | Word/PDF | 检测申请表、报告模板、最终报告 |
| Result Delivery | Application form, Test report | PDF | 检测申请表、检测报告 |
| Data Archiving | Raw data record, Application form, Test report | Paper/PDF | 原始记录、检测申请表、检测报告 |

### 1.3 Risk Hotspots | 风险热点

| Step | Risk Density | Key Risks | Chinese |
|------|--------------|-----------|---------|
| Testing Execution | 8+ risks | Method expired, wrong form, no audit trail, environment exceedance | 方法失效、表格错误、无审计追踪、环境超标 |
| Sample Reception | 4 risks | Quantity mismatch, condition mismatch, transport damage | 数量不符、状态不符、运输损坏 |
| Report Approval | 4 risks | Wrong template, incomplete check, interpretation gap | 模板错误、检查不完整、理解差异 |
| Data Review | 3 risks | Superficial review, no checklist | 审核流于形式、无审核清单 |
| Task Assignment | 3 risks | Unreasonable splitting, insufficient quantity | 分拆不合理、数量不足 |
| Customer Request | 2 risks | Requirement misinterpretation, missing requirements | 需求理解偏差、需求遗漏 |
| Contract Review | 1 risk | Capacity not considered | 未考虑产能 |

### 1.4 System Coverage | 系统覆盖

| Step | Control Method | Status | Chinese |
|------|----------------|--------|---------|
| Customer Request | CRM | Covered | 已覆盖 |
| Contract Review | CRM | Covered | 已覆盖 |
| Sample Reception | LIMS | Covered | 已覆盖 |
| Task Assignment | LIMS | Covered | 已覆盖 |
| Testing Execution | LIMS (partial) + Paper (most) | Mixed | 混合 |
| Data Review | Paper + Manual | Weak | 薄弱 |
| Report Approval | Paper + Manual | Weak | 薄弱 |
| Result Delivery | CRM/LIMS | Covered | 已覆盖 |
| Data Archiving | Paper + Electronic | Mixed | 混合 |

## Layer 2: Root Causes | 原因

### 2.1 Root Causes by Category | 按类别分类的根本原因

| Category | Root Cause | Chinese |
|----------|------------|---------|
| Organizational | Role overlap accepted as necessary for small labs | 小实验室接受角色兼职为必要成本 |
| Organizational | No cross-validation mechanism when roles overlap | 角色兼职时缺少交叉验证机制 |
| Organizational | No independent quality oversight in testing execution | 检测执行无独立质量监督 |
| Cultural | Commercial pressure overrides compliance | 商业压力压倒合规要求 |
| Technical | Paper records lack audit trails and version control | 纸质记录缺乏审计追踪和版本控制 |
| Technical | Excel used for intermediate calculations without control | Excel用于中间计算但不受控 |
| Technical | LIMS not fully trusted for truthful recording | LIMS未被完全信任用于真实记录 |
| Competence | Quality team lacks technical knowledge to review templates | 质量团队缺乏技术知识审核模板 |
| Process | No standardized review checklist | 无标准化审核清单 |
| Process | Template management without content control | 模板管理无内容控制 |

### 2.2 Impact of Each Root Cause | 各根本原因的影响

| Root Cause | Impact Area | Severity | Chinese Impact |
|------------|-------------|----------|----------------|
| Role overlap | Data review, Report approval | High | 数据审核、报告批准 |
| No cross-validation | Quality control | High | 质量控制 |
| No independent oversight | Testing quality | High | 检测质量 |
| Commercial pressure | Sample recording, Reporting | High | 样品记录、报告 |
| Paper lacks controls | Data integrity | High | 数据完整性 |
| Excel uncontrolled | Traceability | High | 可追溯性 |
| LIMS not trusted | Sample lifecycle | High | 样品生命周期 |
| QA lacks knowledge | Report templates | Medium | 报告模板 |
| No review checklist | Data review | Medium | 数据审核 |
| No template content control | Report quality | Medium | 报告质量 |

### 2.3 Key Insight | 关键洞察

| Insight | Chinese |
|---------|---------|
| The fundamental root cause is organizational and cultural, not technical | 根本原因是组织和文化问题，不是技术问题 |
| Systems fail because commercial pressure overrides compliance | 系统失效是因为商业压力压倒合规要求 |
| Role overlap eliminates independent verification | 角色兼职消除了独立验证 |
| Paper and Excel are uncontrolled by nature, not by user error | 纸质和Excel天生失控，不是操作失误 |

## Layer 3: Abstract Model | 抽象模型

### 3.1 Model 1: Role Overlap Risk Matrix | 角色兼职风险矩阵

| Role Overlap | Risk Level | Mitigation | Chinese Mitigation |
|--------------|------------|------------|-------------------|
| Contract Review + Report Approval | High | Monthly sampling cross-check | 每月抽样交叉检查 |
| Data Review + Report Approval | Medium | Separate roles when possible | 尽量分离角色 |
| Sample Admin + Planner | Low | Acceptable | 可接受 |

### 3.2 Model 2: Data Density by Process Step | 流程步骤数据密度

| Step | Data Density | Chinese |
|------|--------------|---------|
| Customer Request | Low | 低 |
| Contract Review | Low | 低 |
| Sample Reception | Medium | 中 |
| Task Assignment | Medium | 中 |
| Testing Execution | Very High | 极高 |
| Data Review | High | 高 |
| Report Approval | High | 高 |
| Result Delivery | Low | 低 |
| Data Archiving | Low | 低 |

### 3.3 Model 3: Control Coverage Continuum | 控制覆盖连续谱

| Tool | Audit Trail | Version Control | Access Control | Integrity Risk | Chinese Risk |
|------|-------------|-----------------|----------------|----------------|--------------|
| Excel | None | None | None | Very High | 极高 |
| Paper | None | Manual | None | High | 高 |
| LIMS | Yes | Yes | Yes | Low | 低 |

### 3.4 Model 4: Risk Ranking by Step | 按步骤风险排序

| Step | Risk Level | Priority | Chinese Priority |
|------|------------|----------|------------------|
| Testing Execution | 5/5 | 1st | 第一优先 |
| Sample Reception | 4/5 | 2nd | 第二优先 |
| Report Approval | 4/5 | 2nd | 第二优先 |
| Data Review | 3/5 | 3rd | 第三优先 |
| Task Assignment | 3/5 | 3rd | 第三优先 |
| Customer Request | 2/5 | 4th | 第四优先 |
| Contract Review | 1/5 | 5th | 第五优先 |

### 3.5 Model 5: Business Pressure vs Recording Behavior | 商业压力与记录行为模型

| Pressure Level | Sample Condition | Typical Behavior | Recording Status |
|----------------|------------------|------------------|------------------|
| Low | Sufficient, stable | Follow process, record truthfully | Trustworthy |
| Medium | Slightly insufficient | Selective recording, internal notes | Partially distorted |
| High |明显不足, customer强势 | Record false in system, keep true on paper | Untrustworthy |
| Very High | Severely insufficient, customer threatening to leave | Fake legitimacy, no trace | Completely distorted |

| 压力等级 | 样品条件 | 典型行为 | 记录状态 |
|----------|----------|----------|----------|
| 低 | 充足、关系稳定 | 按流程走，真实记录 | 可信 |
| 中 | 略不足、客户一般 | 选择性记录，内部备注 | 部分失真 |
| 高 | 明显不足、客户强势 | 系统记假数，纸质留真数 | 不可信 |
| 极高 | 严重不足、丢单即丢客户 | 伪造合理性，不留痕迹 | 完全失真 |

### 3.6 Key Insight | 关键洞察

| Insight | Chinese |
|---------|---------|
| The trustworthiness of sample lifecycle data depends on organizational tolerance for business pressure, not system functionality | 样品生命周期数据的可信度取决于组织对业务压力的承受能力，而不是系统功能 |
| Data integrity = control strength of the tool used | 数据完整性 = 所用工具的控制强度 |
| Highest risk steps need strongest controls | 风险最高的步骤需要最强的控制 |
| When pressure exceeds threshold, systems are bypassed | 当压力超过阈值时，系统会被绕过 |

## Layer 4: Control Logic | 控制逻辑

### 4.1 Control Principles | 控制原则

| Principle | Logic | Chinese |
|-----------|-------|---------|
| Role separation | Reviewer and approver should not be the same person | 审核人与批准人不应为同一人 |
| Cross-validation | When role overlap is unavoidable, add sampling check | 无法避免兼职时增加抽样检查 |
| Data anchoring | Raw data must reference environmental and instrument records | 原始数据必须引用环境和仪器记录 |
| System enforcement | Critical controls should be system-enforced, not manual | 关键控制应由系统强制，而非人工 |
| Risk-based coverage | Highest risk steps need strongest controls | 风险最高的步骤需要最强的控制 |
| Template control | Templates must be centrally managed with version control | 模板必须集中管理并版本控制 |
| Independent review | Quality team must sample-check reports even without technical expertise | 质量团队即使缺乏技术知识也应抽样检查 |
| Truthful recording | Create internal risk notes instead of forcing false records | 创建内部风险备注，而非强制虚假记录 |

### 4.2 Control Points by Step | 按步骤的控制点

| Step | Control Point | Logic | Chinese |
|------|---------------|-------|---------|
| Customer Request | Structured requirement confirmation | Use checklist to capture all requirements | 使用清单捕获所有需求 |
| Contract Review | Capacity verification | Check LIMS capacity calendar before committing | 承诺前检查LIMS产能日历 |
| Sample Reception | Quantity/condition verification | Barcode scan + mandatory upload of anomaly photos | 扫码+异常照片强制上传 |
| Task Assignment | Sample quantity vs method matching | System validates if quantity meets standard requirements | 系统验证样品量是否满足标准要求 |
| Testing Execution | Method version control | Standard library with expiry validation | 标准库+有效期校验 |
| Testing Execution | Record form version control | Centralized template management + force latest version | 模板集中管理+强制使用最新版 |
| Testing Execution | Environmental exceedance interlock | Lock testing when environmental conditions exceed limits | 环境超标时锁定检测 |
| Testing Execution | Audit trail | Unified enable + periodic review | 统一开启+定期审阅 |
| Data Review | Review checklist | Systematized review rules engine | 审核规则引擎 |
| Data Review | Sampling re-check | Randomly sample 10% of records for second review | 随机抽样10%进行二次审核 |
| Report Approval | Template matching | Auto-match template based on contract requirements | 根据合同要求自动匹配模板 |
| Report Approval | Completeness check | System checks signatures, dates, and format before release | 发放前检查签名、日期、格式 |
| Data Archiving | Completeness validation | Pre-archiving checklist | 归档前检查清单 |

### 4.3 Control Classification | 控制分类

| Control Type | Description | Examples | Chinese Examples |
|--------------|-------------|----------|------------------|
| Preventive | Stops errors before they occur | Role separation, template control, capacity verification | 预防性：角色分离、模板控制、产能校验 |
| Detective | Identifies errors after they occur | Sampling re-check, audit trail review, monthly QA sampling | 检测性：抽样复核、审计追踪审阅、月度QA抽样 |
| Corrective | Fixes errors after detection | CAPA process, report correction with version control | 纠正性：CAPA流程、带版本控制的报告修正 |

### 4.4 Control vs Root Cause Mapping | 控制与根因映射

| Root Cause | Primary Control | Secondary Control | Chinese Primary |
|------------|-----------------|-------------------|-----------------|
| Commercial pressure | Internal risk notes (truthful recording alternative) | Escalate to management for risk acceptance | 内部风险备注（替代真实记录） |
| Role overlap | Role separation | Monthly sampling cross-check | 角色分离 |
| Paper lacks controls | Move to LIMS | PDF freeze + controlled distribution | 迁移到LIMS |
| Excel uncontrolled | PDF/A freeze | Hash value for integrity check | PDF/A冻结 |
| QA lacks knowledge | Basic technical training | Focus QA on sampling, not content review | 基础技术培训 |
| No review checklist | Create standardized checklist | Embed in LIMS workflow | 创建标准化清单 |

### 4.5 Key Insight | 关键洞察

| Insight | Chinese |
|---------|---------|
| Control effectiveness depends on whether it addresses the real root cause, not just the symptom | 控制的有效性取决于是否解决了真正的根本原因，而不仅仅是症状 |
| Preventive controls are cheaper than detective or corrective controls | 预防性控制比检测性或纠正性控制成本更低 |
| The best control for commercial pressure is not stronger enforcement, but an alternative truthful path (internal risk notes) | 应对商业压力的最佳控制不是更强的强制，而是替代性的真实路径（内部风险备注） |
| System enforcement is superior to manual control | 系统强制优于人工控制 |

## Layer 5: Data Structure | 数据结构

### 5.1 Core Data Objects | 核心数据对象

| Data Object | Created At | Format | Chinese | Key Fields |
|-------------|------------|--------|---------|------------|
| Test Application Form | Customer Request | Paper/CRM | 检测申请表 | CustomerID, ProductType, TestRequirements |
| Commercial Contract | Contract Review | Paper/CRM | 商业合同 | ContractID, CustomerID, Terms, Price |
| Sample Label | Sample Reception | LIMS/Paper | 样品标签 | SampleID, CustomerID, ProductType, ReceivedDate |
| Sample Storage Record | Sample Reception | LIMS | 样品入库登记 | SampleID, StorageLocation, StorageTime |
| Sample Processing Record | Task Assignment | LIMS/Paper | 样品处理记录 | SampleID, SplitQuantity, ProcessingMethod |
| Task Assignment Record | Task Assignment | LIMS | 任务分派记录 | SampleID, TesterID, AssignedDate, DueDate |
| Raw Data Record | Testing Execution | Paper/LIMS | 原始数据记录表 | RecordID, SampleID, TestStandard, TestResult, InstrumentID |
| Environmental Record | Testing Execution | Paper | 环境记录表 | RecordID, Temperature, Humidity, DateTime |
| Instrument Log | Testing Execution | Paper | 仪器使用记录 | InstrumentID, UserID, StartTime, EndTime, Status |
| Test Report | Report Approval | PDF/Paper | 检测报告 | ReportID, SampleID, Conclusion, PreparedBy, ApprovedBy |

### 5.2 Field Definitions | 字段定义

#### Sample Label | 样品标签

| Field | Type | Required | Chinese | Example |
|-------|------|----------|---------|---------|
| SampleID | String(32) | Yes | 样品编号 | SMP-2026-001234 |
| CustomerID | String(16) | Yes | 客户编号 | CUST-5678 |
| ProductType | Enum | Yes | 产品类型 | Battery / Food / Cosmetic |
| ReceivedDate | Date | Yes | 接收日期 | 2026-06-12 |
| Status | Enum | Yes | 状态 | Received / Pending / InTesting / Tested / Retained / Discarded |

#### Raw Data Record | 原始数据记录表

| Field | Type | Required | Chinese | Example |
|-------|------|----------|---------|---------|
| RecordID | String(32) | Yes | 记录编号 | RAW-2026-001234 |
| SampleID | String(32) | Yes | 样品编号 | SMP-2026-001234 |
| TestStandard | String(64) | Yes | 检测标准 | ISO 17025:2017 |
| TestMethod | String(64) | Yes | 检测方法 | GC-MS-001 |
| TestResult | String(256) | Yes | 检测结果 | 2.5 mg/kg |
| InstrumentID | String(16) | Yes | 仪器编号 | GCMS-01 |
| EnvironmentalCondition | String(128) | No | 环境条件 | Temp:22°C, RH:45% |
| Tester | String(32) | Yes | 检测员 | Zhang San |
| TestDate | Date | Yes | 检测日期 | 2026-06-12 |
| ReviewDate | Date | No | 审核日期 | 2026-06-13 |

#### Test Report | 检测报告

| Field | Type | Required | Chinese | Example |
|-------|------|----------|---------|---------|
| ReportID | String(32) | Yes | 报告编号 | RPT-2026-001234 |
| TemplateID | String(16) | Yes | 模板编号 | TPL-BATTERY-V2 |
| SampleID | String(32) | Yes | 样品编号 | SMP-2026-001234 |
| CustomerID | String(16) | Yes | 客户编号 | CUST-5678 |
| TestStandard | String(64) | Yes | 检测标准 | ISO 17025:2017 |
| TestResult | String(256) | Yes | 检测结果 | Pass / Fail / 2.5 mg/kg |
| Conclusion | Enum | Yes | 判定结论 | Pass / Fail / Inconclusive |
| PreparedBy | String(32) | Yes | 编制人 | Li Si |
| ReviewedBy | String(32) | No | 审核人 | Wang Wu |
| ApprovedBy | String(32) | Yes | 批准人 | Zhao Liu |
| IssueDate | Date | Yes | 签发日期 | 2026-06-15 |
| Version | String(8) | Yes | 版本号 | V1.0 |

### 5.3 Enumerations | 枚举定义

#### Sample Status Enum | 样品状态枚举

| Value | Chinese | Description |
|-------|---------|-------------|
| Received | 已接收 | Sample arrived and logged |
| Pending | 待检 | Waiting for testing |
| InTesting | 检测中 | Currently being tested |
| Tested | 已检 | Testing complete |
| Retained | 留样 | Stored for future use |
| Discarded | 销毁 | Disposed |

#### Report Conclusion Enum | 报告判定枚举

| Value | Chinese | Description |
|-------|---------|-------------|
| Pass | 合格 | Meets all requirements |
| Fail | 不合格 | Does not meet requirements |
| Inconclusive | 不确定 | Cannot determine due to insufficient evidence |

#### Data Status Enum | 数据状态枚举

| Value | Chinese | Description |
|-------|---------|-------------|
| Draft | 草稿 | Initial state, editable |
| Reviewed | 已审核 | Passed review, ready for approval |
| Approved | 已批准 | Approved, ready for freeze |
| Frozen | 已冻结 | Locked, cannot modify |
| Archived | 已归档 | Moved to long-term storage |

### 5.4 Audit Log Structure | 审计日志结构

| Field | Type | Required | Chinese | Description |
|-------|------|----------|---------|-------------|
| LogID | String(32) | Yes | 日志ID | Unique identifier |
| ObjectType | Enum | Yes | 对象类型 | Sample / Data / Report |
| ObjectID | String(32) | Yes | 对象ID | ID of the object being audited |
| Action | Enum | Yes | 操作类型 | Create / Modify / Delete / View / Export / Freeze |
| UserID | String(32) | Yes | 用户ID | Who performed the action |
| Timestamp | DateTime | Yes | 时间戳 | UTC time of the action |
| BeforeValue | JSON | No | 修改前值 | Snapshot before modification |
| AfterValue | JSON | No | 修改后值 | Snapshot after modification |
| ChangeReason | String(256) | No | 修改原因 | Required for Modify/Delete actions |
| IPAddress | String(16) | No | IP地址 | Client IP address |

### 5.5 Key Insight | 关键洞察

| Insight | Chinese |
|---------|---------|
| Data structure must be defined before system implementation | 数据结构必须在系统实施前定义 |
| Enums reduce data entry errors compared to free text | 枚举比自由文本更能减少数据录入错误 |
| Audit log must capture who, what, when, and why | 审计日志必须捕获谁、做了什么、何时、为什么 |
| Cross-references between data objects (SampleID, RecordID, ReportID) enable traceability | 数据对象之间的交叉引用（样品ID、记录ID、报告ID）实现了可追溯性 |
| JSON fields for BeforeValue/AfterValue allow flexible audit logging without rigid schema | 使用JSON字段存储修改前后值，实现灵活的审计日志，无需固定schema |

## Layer 6: State Machine | 状态机

### 6.1 Sample State Machine | 样品状态机

| Current State | Trigger | Next State | Chinese Trigger |
|---------------|---------|------------|-----------------|
| (None) | Sample arrives | Received | 样品到达 |
| Received | Registered | Pending | 登记完成 |
| Pending | Task assigned | Allocated | 任务分派 |
| Allocated | Test started | InTesting | 开始检测 |
| InTesting | Test complete | Tested | 检测完成 |
| Tested | Retain | Retained | 留样 |
| Tested | Discard | Discarded | 销毁 |
| Retained | Expired | Discarded | 留样期满 |

```mermaid
stateDiagram-v2
    [*] --> Received: Sample arrives
    Received --> Pending: Register
    Pending --> Allocated: Assign task
    Allocated --> InTesting: Start test
    InTesting --> Tested: Complete
    Tested --> Retained: Retain
    Tested --> Discarded: Discard
    Retained --> Discarded: Expired
6.2 Sample Exception States | 样品异常状态
Current State	Trigger	Next State	Chinese Trigger
Received	Quantity insufficient	Insufficient	数量不足
Insufficient	Management accepts	RiskAccepted	风险接受
Insufficient	Sample rejected	Rejected	拒绝接收
InTesting	Sample damaged	Damaged	样品损坏
Damaged	No backup	Discarded	无法继续
stateDiagram-v2
    [*] --> Received
    Received --> Insufficient: Quantity below standard
    Insufficient --> RiskAccepted: Management accepts
    Insufficient --> Rejected: Reject sample
    InTesting --> Damaged: Sample damaged
    Damaged --> Discarded: No backup
6.3 Data State Machine | 数据状态机
Current State	Trigger	Next State	Chinese Trigger
(None)	Raw data generated	Draft	数据产生
Draft	Submit	InReview	提交审核
InReview	Reject	Draft	审核不通过
InReview	Approve	Approved	审核通过
Approved	Freeze	Frozen	冻结
Frozen	Archive	Archived	归档
stateDiagram-v2
    [*] --> Draft: Generate raw data
    Draft --> InReview: Submit
    InReview --> Draft: Reject
    InReview --> Approved: Approve
    Approved --> Frozen: Freeze
    Frozen --> Archived: Archive
6.4 Data Exception States | 数据异常状态
Current State	Trigger	Next State	Chinese Trigger
Frozen	Unfreeze request	Unfrozen	申请解冻
Unfrozen	CAPA triggered	CAPA	触发CAPA
stateDiagram-v2
    Frozen --> Unfrozen: Unfreeze request
    Unfrozen --> CAPA: CAPA triggered
6.5 Report State Machine | 报告状态机
Current State	Trigger	Next State	Chinese Trigger
(None)	Draft created	Draft	创建草稿
Draft	Submit	InReview	提交审核
InReview	Reject	Draft	审核不通过
InReview	Approve	Approved	审核通过
Approved	Sign	Signed	签发
Signed	Issue	Issued	发放
Issued	Archive	Archived	归档
Issued	Change request	ChangeRequest	修改申请
ChangeRequest	Change approved	Corrected	修改批准
Corrected	Re-issue	Issued	重新发放
stateDiagram-v2
    [*] --> Draft: Create draft
    Draft --> InReview: Submit
    InReview --> Draft: Reject
    InReview --> Approved: Approve
    Approved --> Signed: Sign
    Signed --> Issued: Issue
    Issued --> Archived: Archive
    Issued --> ChangeRequest: Change request
    ChangeRequest --> Corrected: Approve change
    Corrected --> Issued: Re-issue
6.6 Report Exception States | 报告异常状态
Current State	Trigger	Next State	Chinese Trigger
Issued	Critical error found	Recalled	召回
Recalled	Corrected	Corrected	修正
Recalled	No correction	Obsolete	废弃
stateDiagram-v2
    Issued --> Recalled: Critical error found
    Recalled --> Corrected: Corrected
    Recalled --> Obsolete: No correction
6.7 Cross-Lifecycle Triggers | 跨生命周期触发
Source State	Target State	Trigger	Chinese Trigger
Sample.InTesting	Data.Draft	Raw data generated	产生原始数据
Data.Frozen	Report.Draft	Data ready	数据就绪
Report.Issued	Sample.Retained	Hold for retest	留样备查
flowchart LR
    A[Sample.InTesting] -->|Raw data generated| B[Data.Draft]
    B -->|Data ready| C[Report.Draft]
    C -->|Hold for retest| D[Sample.Retained]
6.8 Key Insight | 关键洞察
Insight	Chinese
State machines make implicit workflow explicit	状态机将隐式的工作流显式化
Exception paths are as important as normal paths	异常路径与正常路径同样重要
Cross-lifecycle triggers connect isolated systems	跨生命周期触发连接孤立的系统


## Layer 7: Minimal Solution | 最小方案

### 7.1 Assumptions | 假设

| Assumption | Chinese |
|------------|---------|
| No new system investment | 不投入新系统 |
| Based on existing tools (LIMS, CRM, paper, Excel) | 基于现有工具（LIMS、CRM、纸质、Excel） |
| Low-cost process changes only | 仅低成本流程变更 |
| Implementation within 3 months | 3个月内可实施 |

### 7.2 Seven Low-Cost Improvements | 七个低成本改进

| # | Improvement | Cost | Effect | Chinese |
|---|-------------|------|--------|---------|
| 1 | Add internal notes field in LIMS for true sample quantity | Very low | Fixes "fear of truthful recording" | LIMS增加内部备注字段记录真实样品量 |
| 2 | Dual-person confirmation for sample check-in/out | Low | Reduces single-person errors | 样品出入库双人确认 |
| 3 | Sample information access log | Low | Enables traceability | 样品信息访问日志 |
| 4 | QA as sole template administrator | Very low | Prevents template chaos | QA为唯一模板管理员 |
| 5 | Template review checklist | Very low | Prevents formatting errors | 模板审核清单 |
| 6 | QA monthly report sampling (5 per month) | Low | Independent oversight | 质量部每月抽样5份报告 |
| 7 | Role separation: preparer ≠ approver | Very low | Independent review | 编制人≠批准人 |

### 7.3 Implementation Priority | 实施优先级

| Priority | Improvement | Reason | Chinese Reason |
|----------|-------------|--------|----------------|
| P1 | #1 Internal notes | Solves core "fear of recording" | 解决核心问题 |
| P1 | #7 Role separation | Fundamental control | 基础控制 |
| P2 | #4 Template centralization | Customer-facing | 客户面对 |
| P2 | #6 QA sampling | Independent oversight | 独立监督 |
| P3 | #3 Access log | Traceability | 可追溯性 |
| P3 | #2 Dual confirmation | Operational | 操作控制 |
| P3 | #5 Template checklist | Preventive | 预防性 |

### 7.4 Detailed Implementation | 详细实施步骤

#### Improvement #1: Internal Notes Field | 内部备注字段

| Step | Action | Chinese | Responsible |
|------|--------|---------|-------------|
| 1 | Add a "InternalNotes" text field to LIMS sample table | 在LIMS样品表中增加"内部备注"文本字段 | LIMS管理员 |
| 2 | Field is visible only to internal staff, not printed on reports | 字段仅内部可见，不打印在报告上 | IT |
| 3 | Train staff to record actual sample quantity when it differs from required | 培训员工在样品量不符时记录真实数量 | QA |
| 4 | Monthly review of internal notes for risk trends | 每月审核内部备注识别风险趋势 | QA Manager |

#### Improvement #2: Dual-Person Confirmation | 双人确认

| Step | Action | Chinese | Responsible |
|------|--------|---------|-------------|
| 1 | Create a paper or digital log for sample check-in/out | 创建样品出入库纸质或电子登记本 | QA |
| 2 | Require two signatures for each sample transaction | 每次样品操作需要两人签名 | Sample Admin |
| 3 | Supervisor to review log weekly for missing signatures | 主管每周审核登记本检查缺失签名 | Lab Supervisor |
| 4 | Include in internal audit checklist | 纳入内审检查表 | QA |

#### Improvement #3: Sample Information Access Log | 样品信息访问日志

| Step | Action | Chinese | Responsible |
|------|--------|---------|-------------|
| 1 | Enable LIMS audit trail for sample record views if available | 如LIMS支持，开启样品记录的审计追踪 | IT |
| 2 | If LIMS does not support, create manual sign-out log for sample files | 如LIMS不支持，创建样品文件借阅登记本 | Sample Admin |
| 3 | Log to capture: who, when, which sample, reason | 登记本记录：谁、何时、哪个样品、原因 | Sample Admin |
| 4 | Quarterly review of access log for unauthorized access | 每季度审核访问日志检查未授权访问 | QA |

#### Improvement #4: QA as Sole Template Administrator | QA为唯一模板管理员

| Step | Action | Chinese | Responsible |
|------|--------|---------|-------------|
| 1 | Collect all report templates currently in use | 收集当前使用的所有报告模板 | QA |
| 2 | Review and consolidate into one master template per report type | 每种报告类型审核并合并为一个主模板 | QA + Technical Manager |
| 3 | Store master templates in read-only shared folder | 将主模板存储在只读共享文件夹 | IT |
| 4 | Restrict write access to QA only | 限制写入权限仅为QA | IT |
| 5 | Any template change requires approval via change request form | 任何模板变更需通过变更申请单批准 | QA |

#### Improvement #5: Template Review Checklist | 模板审核清单

| # | Checklist Item | Chinese |
|---|----------------|---------|
| 1 | Report header contains lab name and logo | 报告页眉包含实验室名称和标志 |
| 2 | Report ID format is consistent | 报告编号格式一致 |
| 3 | Sample ID field is present | 样品编号字段存在 |
| 4 | Customer name/ID field is present | 客户名称/编号字段存在 |
| 5 | Test standard field is present | 检测标准字段存在 |
| 6 | Test method field is present | 检测方法字段存在 |
| 7 | Result field is present | 结果字段存在 |
| 8 | Conclusion (Pass/Fail) field is present | 判定结论字段存在 |
| 9 | Signature lines: Prepared, Reviewed, Approved | 签名栏：编制、审核、批准 |
| 10 | Issue date field is present | 签发日期字段存在 |
| 11 | End line marker (e.g., "*** End of Report ***") is present | 结束线标记存在 |
| 12 | Page numbering is present (X of Y) | 页码存在 |
| 13 | Confidentiality statement is present | 保密声明存在 |
| 14 | Template version number is present | 模板版本号存在 |

#### Improvement #6: QA Monthly Report Sampling | QA每月报告抽样

| Step | Action | Chinese | Responsible |
|------|--------|---------|-------------|
| 1 | QA selects 5 reports randomly from each month's issued reports | QA从每月发放报告中随机抽取5份 | QA |
| 2 | Compare report data against raw data records | 核对报告数据与原始记录 | QA |
| 3 | Check: sample ID, test standard, test method, result, conclusion | 检查项：样品编号、检测标准、检测方法、结果、判定 | QA |
| 4 | Record findings in sampling log | 在抽样记录表中记录发现 | QA |
| 5 | Any discrepancy triggers a non-conformance report | 任何差异触发不符合项报告 | QA |
| 6 | Report monthly summary to lab management | 向实验室管理层报告月度总结 | QA |

#### Improvement #7: Role Separation | 角色分离

| Step | Action | Chinese | Responsible |
|------|--------|---------|-------------|
| 1 | Document in SOP: Preparer and Approver cannot be the same person | 在SOP中写明：编制人和批准人不能为同一人 | QA |
| 2 | If lab has only 2 technical staff, Preparer and Approver must be different | 如实验室只有2名技术员，编制人和批准人必须不同 | Lab Manager |
| 3 | For single-person labs (not recommended), external approver is required | 单人实验室（不推荐），需要外部批准人 | Management |
| 4 | Add to internal audit checklist: verify role separation on reports | 加入内审检查表：核查报告的职责分离 | QA |

### 7.5 Implementation Timeline | 实施时间线

| Week | Actions | Chinese |
|------|---------|---------|
| 1-2 | Improvement #1 (Internal notes) + #7 (Role separation) | 第1-2周：改进#1和#7 |
| 3-4 | Improvement #4 (Template centralization) + #5 (Checklist) | 第3-4周：改进#4和#5 |
| 5-6 | Improvement #2 (Dual confirmation) + #3 (Access log) | 第5-6周：改进#2和#3 |
| 7-8 | Improvement #6 (QA sampling) | 第7-8周：改进#6 |
| 9-10 | Training all staff on new procedures | 第9-10周：培训全体员工 |
| 11-12 | First internal audit of new controls | 第11-12周：首次内审新控制措施 |

### 7.6 Success Criteria | 成功标准

| Criterion | Target | Measurement | Chinese Target |
|-----------|--------|-------------|----------------|
| Template-related audit findings | 50% reduction in 6 months | Compare before/after audit reports | 6个月内模板相关审核发现减少50% |
| Sample quantity discrepancy rate | <5% after 3 months | (Discrepancies / Total samples) × 100% | 3个月后样品数量差异率低于5% |
| Report modification traceability | 100% | % of modifications with change request forms | 100%修改有变更申请单记录 |
| QA sampling completion | 5 reports/month | Count of sampled reports per month | 每月完成5份报告抽样 |
| Role separation compliance | 100% | % of reports with preparer ≠ approver | 100%报告编制人≠批准人 |
| Dual confirmation compliance | 100% | % of sample transactions with two signatures | 100%样品操作有双人确认 |

### 7.7 Key Insight | 关键洞察

| Insight | Chinese |
|---------|---------|
| Minimal solution means minimal cost, not minimal value | 最小方案意味着最小成本，而不是最小价值 |
| Start with P1 improvements that solve core problems | 从解决核心问题的P1改进开始 |
| Process changes are cheaper than system changes but require training | 流程变更比系统变更成本低，但需要培训 |
| Success criteria must be measurable, not vague | 成功标准必须可测量，而非模糊 |
| Even minimal solutions need management commitment | 即使是最小方案也需要管理层的承诺 |