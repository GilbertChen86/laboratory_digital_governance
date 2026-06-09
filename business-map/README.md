
# Laboratory Business Map | 实验室业务全景图

## Overview | 概述

This business map describes the core business process of a testing laboratory, with a focus on the lifecycle management of three key objects: **Samples**, **Data**, and **Reports**. This is the foundation for digital governance.

本业务全景图描述检测实验室的核心业务流程，重点聚焦**样品、数据、报告**三大关键对象的生命周期管理。这是数字治理的基础。

---

## I. Core Business Process | 业务主流程（9 steps | 9步）
Customer Request → Contract Review → Sample Reception → Task Assignment → Testing Execution → Data Review → Report Approval → Result Delivery → Data Archiving

客户需求 → 合同评审 → 样品接收 → 任务分派 → 检测执行 → 数据审核 → 报告批准 → 结果交付 → 数据归档

text

---

## II. Process + Lifecycle Cross-View | 流程 + 三大生命周期交叉视图（Core | 核心）

For each step, this table shows the status and key actions of the three lifecycle objects.

| Step | Sample Lifecycle | Data Lifecycle | Report Lifecycle | Key Roles | Key Control Points |
|------|-----------------|----------------|------------------|-----------|---------------------|
| **Customer Request** | Not exist | Request info created | Not exist | Sales, Customer Service | Requirement confirmation |
| **Contract Review** | Not exist | Contract info created | Not exist | Technical Manager | Capacity verification |
| **Sample Reception** | Created, Stored | Sample info registered | Not exist | Customer Service, Sample Admin | Quantity/condition verification |
| **Task Assignment** | Checked out, Split | Task info bound | Not exist | Sample Admin, Planner | Splitting合理性 |
| **Testing Execution** | Consumed, changed | Raw data generated | Draft created | Tester | Method version, form version, environment, audit trail |
| **Data Review** | Tested | Data under review | In editing | Lab Supervisor/Manager | Review checklist, sampling复核 |
| **Report Approval** | Retained/Discarded | Data reviewed | Final, Approved | Report Compiler, Authorized Signatory | Template matching, integrity check |
| **Result Delivery** | — | — | Issued | Sales, Customer Service | Distribution control |
| **Data Archiving** | Archived | Archived | Archived | Archive Admin | Completeness |

---

## III. Lifecycle State Summary | 三大生命周期状态总览

### Sample Lifecycle | 样品生命周期
Not exist → Received → Pending → In testing → Tested → Retained → Discarded
不存在 → 已接收 → 待检 → 检测中 → 已检 → 留样 → 销毁

text

### Data Lifecycle | 数据生命周期
Request info → Contract info → Sample info → Raw data → Reviewed data → Archived data
需求信息 → 合同信息 → 样品信息 → 原始数据 → 审核数据 → 归档数据

text

### Report Lifecycle | 报告生命周期
Draft → In editing → Final → Approved → Issued → Archived
草稿 → 编辑中 → 正本 → 批准 → 发出 → 归档

text

---

## IV. Role Matrix | 角色与职责矩阵

| Step | Primary Roles | Common Role Overlap Risks |
|------|---------------|---------------------------|
| Customer Request | Sales, Customer Service | Requirement misinterpretation |
| Contract Review | Technical Manager | Overlap with report approval |
| Sample Reception | Customer Service, Sample Admin | — |
| Task Assignment | Sample Admin, Planner | Insufficient technical competence |
| Testing Execution | Tester | — |
| Data Review | Lab Supervisor/Manager | Overlap with approval → superficial review |
| Report Approval | Report Compiler, Authorized Signatory | — |
| Result Delivery | Sales, Customer Service | — |
| Data Archiving | Archive Admin | — |

---

## V. Risk Heatmap | 风险热力图

| Step | Risk Density | Key Risk Count |
|------|--------------|----------------|
| Testing Execution | █████ | 8+ |
| Sample Reception | ████◌ | 4 |
| Report Approval | ████◌ | 4 |
| Data Review | ███◌◌ | 3 |
| Task Assignment | ███◌◌ | 3 |
| Customer Request | ██◌◌◌ | 2 |
| Contract Review | ██◌◌◌ | 1 |
| Result Delivery | ◌◌◌◌◌ | 0 |
| Data Archiving | ◌◌◌◌◌ | 0 |

---

## VI. Current System Coverage | 当前系统覆盖

| Step | Control Method | Status |
|------|----------------|--------|
| Customer Request | CRM | Covered |
| Contract Review | CRM | Covered |
| Sample Reception | LIMS | Covered |
| Task Assignment | LIMS | Covered |
| Testing Execution | LIMS (partial) + Paper (most) | Mixed |
| Data Review | Paper + Manual | Weak |
| Report Approval | Paper + Manual | Weak |
| Result Delivery | CRM/LIMS | Covered |
| Data Archiving | Paper + Electronic | Mixed |

---

## VII. Glossary | 术语表

| Term | Definition |
|------|-------------|
| Sample Lifecycle | The entire process from sample reception to disposal |
| Raw Data | Original records from testing (paper or electronic) |
| Audit Trail | Chronological record of who did what and when |
| Control Point | A step where checks are applied to prevent or detect errors |

| 术语 | 定义 |
|------|------|
| 样品生命周期 | 从样品接收到销毁的完整过程 |
| 原始数据 | 检测产生的最初记录（纸质或电子） |
| 审计追踪 | 按时间顺序记录谁在何时做了什么操作 |
| 控制点 | 用于预防或发现错误的关键环节 |
