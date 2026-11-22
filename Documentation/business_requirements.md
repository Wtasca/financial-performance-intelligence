# Northbridge Building Society
## Business Requirements Document

**Project:** Financial Performance & Profitability Intelligence  
**Project ID:** FPI-001  
**Document Version:** 2.0  
**Organisation:** Fictional UK Building Society  
**Currency:** GBP (£)  
**Financial Year:** April – March

---

## 1. Project Overview

Northbridge Building Society is a fictional regional UK building society with approximately £2.1 billion in assets, £85 million in annual revenue, a £1.5 billion mortgage portfolio and £1.7 billion in savings deposits.

The organisation operates across 12 branches and employs approximately 450 people.

The purpose of this project is to develop a centralised financial performance reporting solution using SQL Server and Power BI.

The solution will consolidate financial information from multiple sources and provide management with a clearer understanding of financial performance, departmental expenditure, budget variances and product profitability.

All company information and financial data used in this project will be synthetic and created for demonstration purposes.

## 2. Business Problem

Northbridge currently relies on fragmented spreadsheets and manual reporting processes to monitor financial performance.

This creates several challenges:

- Financial information is held across multiple sources, making consolidation difficult.
- Management reporting requires significant manual effort.
- Budget variances are not always easy to identify or investigate.
- Departmental expenditure lacks consistent visibility.
- Product profitability is difficult to assess using fragmented financial and portfolio information.
- Management does not have a single reporting environment for monitoring financial performance.

The organisation needs a more consistent and accessible approach to financial reporting.

## 3. Project Objectives

The project aims to:

| ID | Business objective |
|---|---|
| BO01 | Consolidate financial information into a centralised reporting model. |
| BO02 | Provide a clear overview of income, expenses and operating profit. |
| BO03 | Improve visibility of actual financial performance against budget. |
| BO04 | Identify departmental expenditure trends and significant variances. |
| BO05 | Analyse mortgage and savings product performance. |
| BO06 | Reduce manual reporting and improve consistency of financial information. |

## 4. Stakeholders and Business Requirements

The solution will support five main stakeholder groups.

| Stakeholder | Information required | Business objective |
|---|---|---|
| CFO / Finance Director | Overall income, expenses, profitability, financial trends and budget performance | Support strategic financial decisions |
| Financial Controller | Actual versus budget, financial transactions and reporting accuracy | Maintain financial control and reporting reliability |
| Finance Manager | Departmental expenditure, cost trends and budget utilisation | Monitor budgets and manage expenditure |
| Product Manager | Mortgage and savings balances, product income and contribution | Assess product performance and identify opportunities |
| Senior Management | High-level financial performance and key business indicators | Monitor organisational performance and support decisions |

### Key business questions

The solution should help management answer the following questions:

1. How is the organisation performing financially?
2. Is income increasing or decreasing over time?
3. Which expense categories and departments contribute most to expenditure?
4. Are departments operating within their allocated budgets?
5. Which mortgage and savings products contribute most to financial performance?
6. Where are the main opportunities to improve profitability or control costs?

## 5. Project Scope

### In scope

The initial solution will focus on three reporting areas.

| Reporting area | Description | Priority |
|---|---|---|
| Financial Overview | Income, expenses, net interest income, operating profit and financial trends | High |
| Budget vs Actual | Budget performance, departmental expenditure and financial variances | High |
| Product Performance | Mortgage and savings balances, product income and product contribution | High |

### Future enhancements

The following areas may be considered after the initial solution is completed:

- Cash flow analysis.
- Financial forecasting.
- More detailed product pricing and margin analysis.
- Additional cost allocation methods.

### Out of scope

The initial project will not cover:

- Full statutory financial statements.
- IFRS accounting implementation.
- Regulatory capital adequacy calculations.
- Detailed customer-level credit risk or arrears analysis.
- Live integrations with banking systems.
- Regulatory liquidity reporting.

## 6. Functional Requirements

The solution should meet the following requirements.

| ID | Requirement |
|---|---|
| FR01 | Consolidate financial data from multiple structured sources. |
| FR02 | Provide monthly and annual financial reporting. |
| FR03 | Calculate key financial performance indicators consistently. |
| FR04 | Compare actual financial performance against budget. |
| FR05 | Allow analysis of expenditure by department and financial category. |
| FR06 | Provide mortgage and savings product performance analysis. |
| FR07 | Allow users to filter reports by financial year, month, department and product where applicable. |
| FR08 | Provide interactive dashboards with clear visualisations and supporting detail. |

## 7. Dashboard Requirements

The Power BI solution will contain three main dashboards.

### 7.1 Financial Overview

Purpose: Provide management with an overview of the organisation's financial performance.

Key information:

- Total income.
- Total operating expenses.
- Net interest income.
- Operating profit.
- Operating profit margin.
- Monthly and annual performance trends.
- Income and expense breakdowns.

### 7.2 Budget vs Actual

Purpose: Help finance teams monitor financial performance against approved budgets.

Key information:

- Total budget.
- Actual expenditure.
- Budget variance.
- Budget variance percentage.
- Departmental expenditure.
- Expense category breakdown.
- Monthly budget performance.

### 7.3 Product Performance

Purpose: Provide visibility of mortgage and savings product performance.

Key information:

- Mortgage balances.
- Savings balances.
- Product income.
- Product contribution where cost attribution is available.
- Product-level performance comparisons.
- Product portfolio trends.

## 8. Non-Functional Requirements

| ID | Requirement |
|---|---|
| NFR01 | Financial calculations must be accurate and consistently applied. |
| NFR02 | Reports should be easy to navigate and understandable to non-technical users. |
| NFR03 | Typical report interactions should perform efficiently with the synthetic dataset. |
| NFR04 | The data model and reporting solution should be maintainable and allow future enhancements. |

## 9. Data and Technical Requirements

The project will use the following technologies:

| Technology | Purpose |
|---|---|
| Python | Generate and validate synthetic financial datasets |
| SQL Server | Store, transform and analyse financial data |
| SQL | Data preparation, validation and analytical queries |
| Power BI | Data modelling, DAX calculations and interactive dashboards |
| Excel / CSV | Initial data sources and sample datasets |
| GitHub | Version control, project documentation and portfolio presentation |

### Proposed data sources

The synthetic data will represent the following business information:

- General ledger transactions.
- Departmental budgets.
- Mortgage and savings product balances.
- Departmental headcount.

## 10. Acceptance Criteria

The project will be considered successful when:

| ID | Acceptance criterion |
|---|---|
| AC01 | Synthetic financial data is generated for the agreed reporting period. |
| AC02 | Financial data is successfully loaded into SQL Server. |
| AC03 | Data quality checks identify missing, invalid or inconsistent records. |
| AC04 | Financial transactions reconcile to the generated source totals. |
| AC05 | Key financial KPIs are calculated consistently. |
| AC06 | Actual financial performance can be compared against budget. |
| AC07 | Users can analyse financial performance by department and product where applicable. |
| AC08 | Power BI dashboards provide clear and interactive financial reporting. |

## 11. Project Deliverables

| ID | Deliverable |
|---|---|
| D01 | Business Requirements Document |
| D02 | KPI Dictionary |
| D03 | Data Model and Database Architecture |
| D04 | Synthetic Financial Datasets |
| D05 | SQL Database and Analytical Queries |
| D06 | Power BI Financial Performance Dashboards |
| D07 | Business Insights and Recommendations |
| D08 | Project Documentation and GitHub Repository |

## 12. Assumptions and Limitations

- Northbridge Building Society is a fictional organisation.
- All financial data will be synthetically generated.
- The reporting period will cover three completed financial years: April 2023 to March 2026.
- Financial values will be represented in GBP.
- The project is intended to demonstrate BI and financial analysis capabilities rather than replicate a complete banking or accounting system.
- Product profitability will depend on the availability of product-level income and cost attribution.
- The project will use simplified management reporting definitions rather than statutory or regulatory accounting methodologies.

---

**Document status:** Approved project scope for portfolio development.
