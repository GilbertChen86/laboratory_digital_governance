# Project Architecture | 项目架构

## Overview | 概述

This knowledge base is built on a three-layer structure:

本知识库采用三层结构：
┌─────────────────────────────────────────────────────────────────┐
│ LAYER 1: REALITY │
│ 第一层：真实世界 │
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ │
│ │ Phenomena │ │ Audit Finds│ │ Constraints│ │
│ │ 现象 │ │ 审核发现 │ │ 约束条件 │ │
│ └─────────────┘ └─────────────┘ └─────────────┘ │
│ │ │
│ ▼ │
├─────────────────────────────────────────────────────────────────┤
│ LAYER 2: ABSTRACTION │
│ 第二层：抽象模型 │
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ │
│ │ State Models│ │Risk Models │ │DataGovernance│ │
│ │ 状态机 │ │ 风险模型 │ │ 数据治理 │ │
│ └─────────────┘ └─────────────┘ └─────────────┘ │
│ │ │
│ ▼ │
├─────────────────────────────────────────────────────────────────┤
│ LAYER 3: SOLUTION │
│ 第三层：解决方案 │
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ │
│ │ Process │ │ System │ │ Prototypes │ │
│ │ 流程控制 │ │ 系统架构 │ │ 最小原型 │ │
│ └─────────────┘ └─────────────┘ └─────────────┘ │
└─────────────────────────────────────────────────────────────────┘

text

## Module Relationships | 模块关系
┌──────────────────────────────────────────────────────────────────┐
│ Business Map │
│ 业务全景图 │
│ (Process + Roles + Data) │
└──────────────────────────────────────────────────────────────────┘
│
▼
┌──────────────────────────────────────────────────────────────────┐
│ Lifecycle Models (Core) │
│ 生命周期模型（核心） │
│ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ │
│ │ Sample │ │ Data │ │ Report │ │
│ │ 样品 │ │ 数据 │ │ 报告 │ │
│ └──────────────┘ └──────────────┘ └──────────────┘ │
│ │ │ │ │
│ └────────────────┼────────────────┘ │
│ ▼ │
│ ┌──────────┴──────────┐ │
│ │ State Machine Hub │ │
│ │ 状态机总图 │ │
│ └──────────┬──────────┘ │
│ │ │
│ ▼ │
│ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ │
│ │ Instrument │ │ Method │ │ Deviation/ │ │
│ │ 仪器 │ │ 方法 │ │ CAPA │ │
│ └──────────────┘ └──────────────┘ └──────────────┘ │
└──────────────────────────────────────────────────────────────────┘
│
▼
┌──────────────────────────────────────────────────────────────────┐
│ Data Governance │
│ 数据治理框架 │
│ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ │
│ │ ALCOA+ │ │Audit Trail │ │Data Integrity│ │
│ └──────────────┘ └──────────────┘ └──────────────┘ │
└──────────────────────────────────────────────────────────────────┘
│
▼
┌──────────────────────────────────────────────────────────────────┐
│ Risk & Exception Model │
│ 风险与异常模型 │
│ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ │
│ │ Blocking │ │Non-Blocking │ │Risk Levels │ │
│ │ 阻断型 │ │ 非阻断型 │ │ 风险等级 │ │
│ └──────────────┘ └──────────────┘ └──────────────┘ │
└──────────────────────────────────────────────────────────────────┘
│
▼
┌──────────────────────────────────────────────────────────────────┐
│ Digital Control Architecture │
│ 数字化控制架构 │
│ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ │
│ │ Process │ │ System │ │ Roadmap │ │
│ │ 流程控制 │ │ 系统规划 │ │ 路线图 │ │
│ └──────────────┘ └──────────────┘ └──────────────┘ │
└──────────────────────────────────────────────────────────────────┘

text

## Content Layering per Module | 模块内容分层

For each module, content follows this 7-layer structure:

每个模块的内容按以下七层结构组织：

| Layer | Name | Description |
|-------|------|-------------|
| 1 | Phenomena | What actually happens in the lab |
| 2 | Root Causes | Why it happens |
| 3 | Abstract Model | The pattern or law behind the phenomena |
| 4 | Control Logic | How to control it |
| 5 | Data Structure | How to structure it (fields, enums, logs) |
| 6 | State Machine | State transitions |
| 7 | Minimal Solution | Lowest-cost actionable implementation |

| 层 | 名称 | 描述 |
|----|------|------|
| 1 | 现象 | 实验室实际发生了什么 |
| 2 | 原因 | 为什么发生 |
| 3 | 抽象模型 | 现象背后的规律或模式 |
| 4 | 控制逻辑 | 如何控制 |
| 5 | 数据结构 | 如何结构化（字段、枚举、日志） |
| 6 | 状态机 | 状态转换 |
| 7 | 最小方案 | 最低成本的可执行落地方案 |

## Directory Structure | 目录结构
laboratory_digital_governance/
├── README.md # Project overview
├── business-map/ # Business process + roles + data objects
├── lifecycle-model/ # Lifecycle models for key objects
│ ├── sample-lifecycle.md
│ ├── data-lifecycle.md
│ ├── report-lifecycle.md
│ ├── instrument-lifecycle.md
│ └── capa-lifecycle.md
├── data-governance/ # ALCOA+, metadata, data integrity
├── audit-trail/ # Audit trail management
├── risk-model/ # Risk and exception classification
├── state-machine/ # State machine diagrams (unified)
├── architecture/ # Digital control architecture
├── diagrams/ # Visual models (this file)
├── prototypes/ # Templates, checklists, SOP snippets
└── articles/ # Industry insight articles

text