> **Real-World Project — data and company name changed to protect sensitive information**
> Developed for telecommunications operator — to give
> C-level leadership real-time visibility over a complex, multi-year infrastructure investment
> program. Financial figures and project identifiers in this repository have been replaced with
> representative demo data for public sharing. The architecture, hierarchy design, KPI logic,
> and DAX measures are identical to the production dashboard in active use.

# 💼 Enterprise Budget Management Dashboard

[![Power BI](https://img.shields.io/badge/Power%20BI-Pro-yellow.svg)](https://powerbi.microsoft.com/)
[![Status](https://img.shields.io/badge/Status-Production-success.svg)]()
[![License](https://img.shields.io/badge/License-MIT-blue.svg)]()

> **Providing C-level executives with real-time visibility over an $84M annual infrastructure program — from portfolio-level budget execution to individual contract milestones.**

![Dashboard Preview](./assets/preview.png)

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Dashboard Pages](#-dashboard-pages)
- [Dashboard Construction Process](#-dashboard-construction-process)
- [Business Context](#-business-context)
- [Development Process](#-development-process)
- [Technical Outcomes](#-technical-outcomes)
- [Lessons Learned](#-lessons-learned)

---

## 🎯 Project Overview

A **four-level executive intelligence platform** built in Power BI to consolidate financial and operational $84M annual infrastructure investment program. The dashboard gives C-level leadership and program directors a single, authoritative view across:

- 🏗️ **Portfolio Level** — Total program budget execution and overall financial health
- 📂 **Program Level** — Budget vs. actual breakdown across program groups
- 📌 **Project Level** — Individual project performance: cost variance, execution rate, schedule status
- 📄 **Contract Level** — 104 active procurement contracts: milestones, payments, risk flags

Before this system, consolidating portfolio-level financial data required manual extraction from disconnected sources — a process taking 5+ hours per weekly reporting cycle. The dashboard collapsed that to an automated, real-time view available to authorized stakeholders at any time.

### Quick Stats

| Metric | Value |
|--------|-------|
| **Annual Program Budget** | $84M+ |
| **Active Projects** | 16 |
| **Contracts Monitored** | 104 |
| **Dashboard Pages** | 4 |
| **Hierarchy Levels** | Portfolio → Program → Project → Contract |

---

## ⚡ Key Features

- ✅ **Four-Level Drill-Through** — Navigate from portfolio summary to individual contract in four clicks
- 📊 **Budget vs. Actual Analysis** — Real-time execution rate and variance at every hierarchy level
- 🚦 **Traffic Light Indicators** — Instant visual flags for projects at risk of under- or over-execution
- 📈 **Period-over-Period Trends** — Spending velocity and execution trajectory analysis
- 🔐 **Role-Based Access Control** — Row-level security aligned to the organizational hierarchy
- ⚡ **Automated Daily Refresh** — Power BI Service with scheduled refresh, no manual intervention
- 📱 **Executive-Optimized Design** — Clean KPI cards, minimal visual noise, decision-ready layout
- 📤 **Export-Ready Reporting** — Formatted outputs for board presentations and regulatory review

---

## 📊 Dashboard Pages

### 1️⃣ Portfolio Executive Overview

**Purpose**: Give C-level leadership a single-screen financial health summary for the entire $84M program.

![](./screenshots/1portfolio_executive_overview.png)

**Key Visualizations**:
- **Budget Execution Rate KPI Card** — Overall program spending vs. plan, with tolerance band
- **Project Health Matrix** — Traffic light summary across all 16 active projects
- **Spending Trend Line** — Period-over-period budget execution velocity
- **Variance by Program Group** — Horizontal bar chart identifying which programs are ahead or behind plan

**Executive Value**: Enables the CEO and CFO to assess the health of the entire investment program in under 30 seconds, without requiring input from program directors.

---

### 2️⃣ Program Performance

**Purpose**: Break down budget execution and schedule performance across the program groups within the portfolio.

![](./screenshots/2program_performance.png)

**Key Metrics**:
- Budget execution rate per program group
- Cost variance (absolute and percentage)
- Number of projects within each program, by health status
- Period-over-period variance trend

**Key Visualizations**:
- Multi-row KPI cards per program
- Budget vs. actual waterfall chart
- Schedule performance comparison matrix
- Drill-through to Project Detail enabled from every row

**Business Impact**: Allows the Program Director to identify which program areas require immediate financial intervention before the weekly executive review.

---

### 3️⃣ Project Detail

**Purpose**: Provide project-level financial and schedule performance for each of the 16 active projects.

![](./screenshots/3project_detail.png)

**Key Metrics**:

| Column | Description |
|--------|-------------|
| **Project** | Project name (anonymized in public repo) |
| **Budget** | Allocated project budget |
| **Actual Spend** | Cumulative spending to date |
| **Execution Rate** | Actual ÷ Budget (%) |
| **Variance** | Budget − Actual (absolute value) |
| **Status** | On Track / At Risk / Critical |
| **Contracts** | Number of active contracts linked |

**Key Visualizations**:
- Project performance table with conditional formatting and traffic light column
- Execution rate gauge per project
- Variance distribution chart across the 16-project portfolio
- Contract count per project (linked to Contract Tracking page via drill-through)

**Business Impact**: Gives project managers and program directors a precise view of financial standing before weekly status meetings.

---

### 4️⃣ Contract & Procurement Tracking

**Purpose**: Monitor the 104 active procurement contracts: payment milestones, execution status, and risk flags.

![](./screenshots/4contract_procurement.png)

**Key Metrics**:
- Contracts by procurement stage
- Payment milestone completion rate
- Contracts flagged at risk (execution below threshold or past milestone date)
- Spending distribution by contract type

**Key Visualizations**:
- Contract pipeline by procurement stage (funnel or bar)
- Milestone calendar heatmap
- At-risk contract alert table with conditional formatting
- Spending breakdown by contract type and procurement category

**Business Impact**: Provides the procurement and legal teams with a live view of contract risk exposure across the full program.

---

## 👨‍💼 Dashboard Construction Process

Every design decision was governed by a single question: *What does C-level Management need to see before the weekly executive review?*

### Strategic Planning
- 🎯 Defined four-level hierarchy (Portfolio → Program → Project → Contract) based on Company's organizational and governance structure
- 📋 Designed KPI framework aligned to the investment program's financial reporting requirements
- 🔄 Validated metric definitions with program finance and procurement teams before development began

### Technical Execution
- 🛠️ **End-to-end Power BI development** — from data modeling to production deployment
- 📊 Multi-source data consolidation from project management, financial, and procurement systems
- 💻 DAX measure library for budget variance, execution rates, period-over-period analysis, and risk indicators
- 🔍 Performance optimization for automated daily refresh with live operational data

### Deployment
- 🚀 Published to Company's Power BI Service organizational workspace
- 🔐 Row-level security configured for four organizational access levels
- 📅 Automated daily refresh aligned to the financial reporting calendar
- 📚 User documentation and executive navigation guide

---

## 💼 Business Context

The Company manages one of the most complex investment programs in Ecuador's public sector: 16 concurrent infrastructure projects, 104 procurement contracts, and an $84M annual budget — all subject to Ecuador's SERCOP public procurement regulations. The reporting challenge this dashboard was designed to solve is structural, not incidental.

### The Problem Before This Dashboard

| Area | Before | After |
|---|---|---|
| **Reporting cycle** | 5+ hours of manual extraction weekly | Real-time, automated, always current |
| **Data sources** | 3 disconnected systems (financial, SERCOP, MS Project) | Single consolidated Power BI model |
| **Visibility level** | Portfolio totals only | Portfolio → Program → Project → Contract |
| **Distribution** | Manual PDF via email | Self-service access for authorized stakeholders |
| **Risk identification** | Discovered in meetings | Live traffic light flags, visible before meetings |

### The Questions It Was Built to Answer

- Is the $84M portfolio on track to execute within budget and schedule tolerance?
- Which of the 16 active projects are behind plan — and by how much?
- Which of the 104 contracts are at risk of payment delays or milestone slippage?
- How does current-period execution compare to plan at each of the four hierarchy levels?
- What does the CFO need to see before the weekly executive review — in one screen?

These questions are not unique to the current project or Company. They are the standing financial governance agenda of any large infrastructure operator, utility, or public investment program.

---

## 🔧 Development Process

### Phase 1: Requirements & Architecture Design (Week 1–2)

**Activities**:
- Defined four-level data hierarchy aligned to Company's organizational and reporting structure
- Established KPI dictionary: budget execution rate, cost variance, schedule performance
- Designed page wireframes for all four dashboard views

**Deliverables**:
- KPI specification document with metric definitions and calculation logic
- Data model architecture diagram
- Dashboard wireframes (4 pages) validated with program directors

---

### Phase 2: Data Integration & Modeling (Week 3–4)

**Activities**:
- **Data Sources**: Budget data from internal financial systems; contract data from SERCOP (Ecuador's national public procurement platform); project schedule data from MS Project exports
- **ETL Development**: Power Query M transformations for data cleansing, currency normalization, and fiscal period alignment across sources
- **Data Modeling**: Star schema supporting four-level drill-through hierarchy
- **Quality Assurance**: Power BI totals reconciled line-by-line against source financial records

**Data Model Structure**:
```
├── Fact_BudgetExecution  — period-level planned vs. actual spend
├── Fact_Contracts        — contract-level tracking (104 contracts)
├── Dim_Project           — 16 projects with program assignment and metadata
├── Dim_Program           — program group hierarchy
├── Dim_Time              — fiscal period calendar with MTD/YTD logic
└── Dim_ContractStatus    — procurement stage and risk classification lookup
```

**Tools & Techniques**:
- Power Query M for multi-source ETL and period alignment
- DAX for financial KPIs, variance calculations, and time intelligence

---

### Phase 3: Dashboard Development (Week 5–7)

#### Core DAX Measures
```DAX
Budget Execution Rate = 
DIVIDE(
    [Total Actual Spend],
    [Total Budgeted Amount],
    0
) * 100

Cost Variance = 
[Total Actual Spend] - [Total Budgeted Amount]

Cost Variance % = 
DIVIDE(
    [Cost Variance],
    [Total Budgeted Amount],
    0
) * 100

Projects At Risk = 
CALCULATE(
    COUNTROWS(Dim_Project),
    Dim_Project[Status] = "At Risk"
        || Dim_Project[Status] = "Critical"
)

Period Execution Velocity = 
DIVIDE(
    CALCULATE([Total Actual Spend], DATESMTD(Dim_Time[Date])),
    CALCULATE([Total Budgeted Amount], DATESMTD(Dim_Time[Date])),
    0
) * 100
```

**Visualizations Created**:
- Executive KPI cards with traffic light conditional formatting
- Waterfall charts for budget vs. actual variance at each hierarchy level
- Four-level drill-through navigation (portfolio → program → project → contract)
- Contract milestone calendar heatmap
- At-risk project and contract alert tables

---

### Phase 4: Testing & Validation (Week 8)

**Financial Reconciliation**:
- All Power BI totals validated against source financial system records
- Variance calculations cross-checked against the existing manually produced Excel baseline
- Drill-through filter context verified at all four hierarchy levels — context must propagate correctly from portfolio level to individual contract

**Design Refinement**:
- Reduced visual complexity per page through review with program directors
- Simplified executive overview to 5 core KPIs for C-level viewing
- Added navigation breadcrumbs for drill-through orientation (critical for non-technical users)

---

### Phase 5: Production Deployment (Week 9–10)

**Deployment**:
- Published to Company's Power BI Service organizational workspace
- Row-level security configured for four organizational access levels
- Automated daily refresh established, aligned to the financial reporting calendar

**Documentation**:
- Executive user guide with navigation and metric interpretation instructions
- Technical documentation: data model diagram, DAX measure library, refresh configuration

---

## 📈 Technical Outcomes

### Architecture Achievement: Four-Level Drill-Through

The core technical challenge was building a single coherent data model that supports seamless navigation from an $84M portfolio summary down to an individual contract milestone — without performance degradation at any level.

| Level | Table | Primary DAX Context | Key KPIs |
|---|---|---|---|
| **Portfolio** | Dim_Program (all) | No filter | Execution Rate, Total Variance, Projects At Risk |
| **Program** | Dim_Program (filtered) | CALCULATE with program filter | Program-level BvA, Project Count |
| **Project** | Dim_Project | CALCULATE with project filter | Cost Variance %, Execution Rate, Contract Count |
| **Contract** | Fact_Contracts | CALCULATE with contract filter | Milestone Status, Payment Execution, Risk Flag |

The model uses a snowflake structure with `Dim_Program` bridging `Dim_Project` to the portfolio level, combined with `USERELATIONSHIP` for cross-level aggregations where needed.

---

### Multi-Source ETL Architecture

Three data sources with different structures, identifiers, and update frequencies consolidated into a single coherent model:

```
SERCOP (procurement platform)   →  Fact_Contracts
                                   Contract IDs, milestones, payment schedules
                                   
Internal financial system       →  Fact_BudgetExecution
                                   Period-level planned vs. actual spend
                                   
MS Project (schedule exports)   →  Dim_Project status fields
                                   Timeline status, milestone flags
```

**Key ETL design decisions**:
- Master mapping table linking internal project codes to SERCOP contract IDs — built in Phase 1
- Fiscal period normalization: each source uses a different period boundary convention
- Incremental refresh for `Fact_BudgetExecution` to manage daily update volume

---

### DAX Measure Library

Budget and variance analysis:
- Budget Execution Rate, Cost Variance (absolute and %), Period Execution Velocity
- YTD Execution Rate, MTD Variance, Prior Period Comparison

Risk and status indicators:
- Projects At Risk, Critical Project Flag, At-Risk Contract Alert
- Traffic light logic via SWITCH for conditional formatting across all four pages
- Drill-through filter context preservation at each hierarchy level

Time intelligence:
- MTD, YTD, and prior-period calculations using DATESMTD, DATESYTD, SAMEPERIODLASTYEAR
- Period-over-period velocity: how fast is execution accelerating or decelerating?

---

### Executive Dashboard Design Principles

| Design Decision | Rationale |
|---|---|
| Maximum 5 KPIs on executive overview | A CFO's review time is under 5 minutes; everything must be immediately actionable |
| Traffic light system, not trend charts, on overview | Executives need a clear threshold answer, not a data exploration challenge |
| Drill-through over cross-page filters | Preserves context at each level; filters alone lose hierarchy orientation |
| Breadcrumb navigation at each drill-through level | Non-technical executives cannot orient themselves without visual confirmation of where they are |
| Neutral government-sector color palette | Avoids visual noise; consistent with Company's internal reporting conventions |

---

## 💡 Lessons Learned

### Technical Insights

#### 1. **Multi-Source Integration Requires a Master Key — Built in Phase 1**
**Challenge**: Three data sources used different identifiers for the same projects and contracts, with no natural join key.

**Solution**:
- Built a master mapping table linking internal project codes to SERCOP contract IDs in the first week of development
- Implemented lookup validation in Power Query to surface unmapped records before load — making data quality issues visible, not hidden

**Lesson**: The effort to build a master mapping table in Phase 1 is trivial compared to rebuilding the model in Phase 4 when mismatches surface in production. Establish it first.

---

#### 2. **Executive Dashboards Must Work Without the Developer in the Room**
**Challenge**: An executive-facing dashboard will be used in board meetings and CFO reviews — environments where no developer is present and no explanation is available.

**Solution**:
- Added navigation breadcrumbs at each drill-through level showing current hierarchy position
- Used consistent visual language (same chart types at equivalent hierarchy levels)
- Provided a single-page printed navigation reference alongside the digital dashboard

**Lesson**: Treat the first solo use by a non-technical executive as the acceptance test. If a CFO can navigate four hierarchy levels without guidance, the design is correct.

---

#### 3. **Financial Dashboards Must Prove Correctness — Not Assume It**
**Challenge**: Initial Power BI totals did not exactly match the existing manually produced Excel reports, creating trust issues with the finance team that threatened adoption.

**Solution**:
- Conducted line-by-line reconciliation between Power BI and all three source systems
- Identified three discrepancies caused by period-boundary logic in the ETL pipeline
- Established an automated daily reconciliation check as part of the refresh process — a permanent fixture, not a one-time fix

**Lesson**: For financial dashboards, correctness is not assumed — it must be demonstrated through reconciliation before any executive sees the output. A single unexplained variance costs more in trust than months of correct figures restore.

---

#### 4. **Automated Refresh Requires Resilient ETL — Not Demo ETL**
**Challenge**: Automated daily refresh surfaced data quality issues (null contract IDs, period mismatches, missing project codes) that were invisible during manual development with clean data.

**Solution**:
- Added explicit error handling in Power Query for all known data quality failure modes
- Configured Power BI Service email alerts for refresh failures
- Implemented a data quality pre-check step at the start of each refresh cycle — surfacing issues before they reach the dashboard

**Lesson**: Build ETL pipelines assuming the worst-quality input on every refresh cycle. A pipeline that works reliably on clean demo data will fail in production.

---

## 🔖 Tags

`power-bi` `data-analytics` `business-intelligence` `project-management` `pmo` `budget-management` `kpi-dashboard` `dax` `power-query` `etl` `data-modeling` `executive-dashboard` `infrastructure` `telecommunications` `government` `procurement`

---

<div align="center">

**⭐ If you find this project useful, please consider giving it a star! ⭐**

Made with ❤️ and ☕ by Fernando Munoz

[⬆ Back to Top](#-enterprise-budget-management-dashboard)

</div>
