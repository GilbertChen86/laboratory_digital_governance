Project Architecture | 项目架构
Overview | 概述
This knowledge base is built on a three-layer structure:

本知识库采用三层结构：

flowchart TD
    subgraph L1 [LAYER 1: REALITY - 第一层：真实世界]
        Phenomena[Phenomena<br>现象]
        Audit[Audit Finds<br>审核发现]
        Constraints[Constraints<br>约束条件]
    end

    subgraph L2 [LAYER 2: ABSTRACTION - 第二层：抽象模型]
        StateModels[State Models<br>状态机]
        RiskModels[Risk Models<br>风险模型]
        DataGov[Data Governance<br>数据治理]
    end

    subgraph L3 [LAYER 3: SOLUTION - 第三层：解决方案]
        Process[Process Control<br>流程控制]
        System[System Architecture<br>系统架构]
        Prototypes[Prototypes<br>最小原型]
    end

    L1 --> L2 --> L3
Module Relationships | 模块关系
flowchart TD
    BM[Business Map<br>业务全景图]
    
    subgraph LCM [Lifecycle Models - Core<br>生命周期模型（核心）]
        Sample[Sample<br>样品]
        Data[Data<br>数据]
        Report[Report<br>报告]
    end
    
    SMH[State Machine Hub<br>状态机总图]
    
    subgraph LCM2 [Lifecycle Models - Extended<br>生命周期模型（扩展）]
        Instrument[Instrument<br>仪器]
        Method[Method<br>方法]
        CAPA[Deviation/CAPA<br>偏差/CAPA]
    end
    
    DG[Data Governance<br>数据治理框架]
    REM[Risk & Exception Model<br>风险与异常模型]
    DCA[Digital Control Architecture<br>数字化控制架构]
    
    BM --> LCM
    Sample --> SMH
    Data --> SMH
    Report --> SMH
    SMH --> LCM2
    LCM2 --> DG
    DG --> REM
    REM --> DCA
Content Layering per Module | 模块内容分层
For each module, content follows this 7-layer structure:

每个模块的内容按以下七层结构组织：

Layer	Name	Description
1	Phenomena	What actually happens in the lab
2	Root Causes	Why it happens
3	Abstract Model	The pattern or law behind the phenomena
4	Control Logic	How to control it
5	Data Structure	How to structure it (fields, enums, logs)
6	State Machine	State transitions
7	Minimal Solution	Lowest-cost actionable implementation
层	名称	描述
1	现象	实验室实际发生了什么
2	原因	为什么发生
3	抽象模型	现象背后的规律或模式
4	控制逻辑	如何控制
5	数据结构	如何结构化（字段、枚举、日志）
6	状态机	状态转换
7	最小方案	最低成本的可执行落地方案
Directory Structure | 目录结构
text
laboratory_digital_governance/
├── README.md                    # Project overview
├── business-map/                # Business process + roles + data objects
├── lifecycle-model/             # Lifecycle models for key objects
│   ├── sample-lifecycle.md
│   ├── data-lifecycle.md
│   ├── report-lifecycle.md
│   ├── instrument-lifecycle.md
│   └── capa-lifecycle.md
├── data-governance/             # ALCOA+, metadata, data integrity
├── audit-trail/                 # Audit trail management
├── risk-model/                  # Risk and exception classification
├── state-machine/               # State machine diagrams (unified)
├── architecture/                # Digital control architecture
├── diagrams/                    # Visual models (this file)
├── prototypes/                  # Templates, checklists, SOP snippets
└── articles/                    # Industry insight articles