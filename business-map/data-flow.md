markdown
# Data Flow Diagram | 数据流向图

## Core Data Objects and Their Flow | 核心数据对象及其流转

| Data Object | Created At | Used At | Archived At | Format |
|-------------|------------|---------|-------------|--------|
| Test Application Form | Customer Request | Contract Review, Sample Reception, Task Assignment, Data Review, Result Delivery | Data Archiving | Paper/CRM |
| Sample Label | Sample Reception | Task Assignment, Testing Execution | Data Archiving | LIMS/Paper |
| Raw Data Record | Testing Execution | Data Review, Report Approval | Data Archiving | Paper/LIMS |
| Environmental Record | Testing Execution | Data Review | Data Archiving | Paper |
| Instrument Log | Testing Execution | Data Review | Data Archiving | Paper |
| Test Report | Report Approval | Result Delivery, Data Archiving | Data Archiving | PDF/Paper |

---

## Data-to-System Mapping | 数据与系统映射

| System | Data Objects |
|--------|---------------|
| CRM | Test application form, commercial contract |
| LIMS | Sample label, storage records, partial raw data |
| Paper | Environmental records, instrument logs, most raw data, signed report copies |
| Excel | Data cleaning, intermediate calculations (uncontrolled area) |

---

## Data Traceability Example | 数据追溯路径示例

**From final report back to raw data:**
Test Report
↓ (Report Number)
Test Application Form
↓ (Sample ID)
Raw Data Record
↓
Instrument Log / Environmental Record

text

**从最终报告反向追溯到原始数据：**
检测报告
↓（报告编号）
检测申请表
↓（样品编号）
原始数据记录表
↓
仪器使用记录 / 环境记录

text

---

## Notes | 说明

- The uncontrolled use of Excel for intermediate calculations is a major data integrity risk.
- Paper records lack audit trails and version control.
- Future improvements should focus on bringing paper and Excel under governance.

- Excel用于中间计算且不受控，是数据完整性的主要风险点。
- 纸质记录缺乏审计追踪和版本控制。
- 未来的改进应聚焦于将纸质和Excel纳入治理范围。