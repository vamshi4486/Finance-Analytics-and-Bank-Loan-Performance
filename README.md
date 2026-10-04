# Finance Analytics & Bank Loan Performance

A data analytics project focused on exploring **bank loan and customer financial data** using **Microsoft Excel** for source data management and **Microsoft Power BI** for data analysis, visualization and interactive reporting.

## Project Overview

This project analyzes customer bank-loan data using two Excel datasets, `Finance_1.xlsx` and `Finance_2.xlsx`, each containing more than 39,000 records, as specified in the project presentation. The Power BI report explores loan amounts, revolving balances, payment activity, verification status, loan status across states and months, and home ownership in relation to last payment dates.

> **Data note:** Use only synthetic, anonymized or otherwise authorized data in this public repository. Do not upload real customer-identifiable, confidential or restricted financial information.

## Problem Statement

Financial loan datasets contain large volumes of information about loan amounts, borrower attributes, credit history, verification status, loan status and repayment activity. When records are maintained across multiple Excel workbooks, it can be difficult to review the data consistently and understand how loan portfolio measures vary across time, geography and customer segments.

This project addresses the need for a consolidated, interactive analytical view of the bank-loan data. Microsoft Power BI is used to organize relevant loan and repayment attributes into report visuals and KPI areas, allowing users to explore year-wise loan amounts, revolving balances by grade and sub-grade, payment totals by verification status, loan status by state and month, and last payment dates across home ownership categories. The report supports descriptive analysis and exploration, not credit scoring or automated lending decisions.

## Tools & Technologies

- **Microsoft Power BI** — data modeling, measures, interactive dashboards and reporting
- **Microsoft Excel** — source datasets and data inspection
- **Power Query** — data transformation and preparation, if used in the report
- **DAX** — calculated measures and KPIs, if used in the report
- **Git & GitHub** — version control and project sharing

## Repository Structure

```text
Finance-Analytics-and-Bank-Loan-Performance/
├── README.md
├── .gitignore
├── LICENSE
├── Data/
│   └── Raw/
│       ├── Finance_1.xlsx
│       └── Finance_2.xlsx
├── PowerBI/
│   ├── Finance_Project.pbix
│   └── Screenshots/
│       └── README.md
├── Documentation/
│   ├── Project_Documentation.md
│   └── Data_Dictionary.md
└── Project Brief/
    └── Project_Bootcamp.pptx
```

## Data Sources

| Dataset | Description |
|---|---|
| `Finance_1.xlsx` | Loan details, borrower attributes, loan grades, verification status, loan status and geographic information |
| `Finance_2.xlsx` | Credit history, revolving balances, repayment details, outstanding principal and payment dates |

Both observed workbook headers contain a common `id` field. Validate uniqueness, missing values and matching records before using it to relate the datasets.

## Key Fields

| Field | Purpose |
|---|---|
| `id` | Loan or record identifier |
| `loan_amnt` | Loan amount |
| `funded_amnt` | Funded loan amount |
| `funded_amnt_inv` | Amount funded by investors |
| `grade` / `sub_grade` | Loan grade categories |
| `home_ownership` | Home ownership category |
| `verification_status` | Verification category |
| `issue_d` | Loan issue date |
| `loan_status` | Loan status |
| `addr_state` | State associated with the record |
| `revol_bal` | Revolving balance |
| `total_pymnt` | Total payment amount |
| `last_pymnt_d` | Last payment date |
| `last_pymnt_amnt` | Last payment amount |

See `Documentation/Data_Dictionary.md` for observed source fields.

## Project Objectives

1. Analyze year-wise loan amount statistics.
2. Explore revolving balances across loan grades and sub-grades.
3. Compare total payments for verified and non-verified statuses.
4. Analyze loan status across states and months.
5. Explore home ownership categories in relation to last payment dates.
6. Present loan portfolio information through interactive Power BI reports.

## Key Performance Indicators (KPIs)

| KPI | Description |
|---|---|
| Year-wise Loan Amount Stats | Analyze loan amounts across years |
| Grade and Sub-grade-wise Revolving Balance | Explore revolving balances by loan grade and sub-grade |
| Verified vs. Non-Verified Total Payment | Compare total payments across verification groups |
| State-wise and Month-wise Loan Status | Explore loan status across geographic and monthly categories |
| Home Ownership vs. Last Payment Date | Analyze last payment dates across home ownership groups |

Verify exact aggregation, filters, date fields and DAX definitions from the final PBIX before documenting specific calculations.

## Project Workflow

1. **Data collection:** Use the two supplied Excel workbooks.
2. **Data inspection:** Review workbook structures, column names, data types, record counts and sample records.
3. **Data preparation:** Review missing values, duplicate identifiers, inconsistent categories and date formats.
4. **Data validation:** Validate the common `id` field, numeric values, date fields and matching records.
5. **Data modeling:** Configure Power BI tables and relationships based on validated keys.
6. **Data analysis:** Prepare measures and aggregations for the project KPIs.
7. **Visualization:** Develop interactive visuals for loan amounts, revolving balances, payments, loan status and home ownership.
8. **Report validation:** Verify totals, filters, slicers, relationships and visual interactions.
9. **Documentation:** Record the actual data preparation, model, KPI definitions and limitations.

The workflow includes recommended stages; document only transformations and checks actually completed in the report.

## Data Quality Checks

Review for:
- Null, blank and missing values
- Duplicate loan or record identifiers
- Inconsistent data types and date formats
- Unexpected numeric values in loan and payment fields
- Inconsistent grade, sub-grade, verification and loan-status categories
- Missing or unmatched identifiers between workbooks
- Unusual or incomplete repayment information

Record which checks were actually performed and which issues were corrected.

## Getting Started

### Requirements
- Microsoft Power BI Desktop
- Microsoft Excel or a compatible spreadsheet application
- Source workbooks, if required to refresh the report
- Git (optional)

### Open the Power BI Report
1. Clone or download this repository.
2. Open `PowerBI/Finance_Project.pbix` in Power BI Desktop.
3. Configure data source paths if prompted.
4. Review the data model, relationships, measures and report pages.
5. Refresh the report if the source files and connections are configured.
6. Verify that visuals and KPI calculations load correctly.

The PBIX may require updated source paths when opened on another computer.

## Results

The repository contains the Power BI report and documentation for exploring the KPI areas identified in the project brief. Add sanitized screenshots, verified numerical findings and business observations after reviewing and validating the final report.

## Limitations & Responsible Use

- This is a financial data analytics portfolio project, not a credit-scoring or automated loan-approval system.
- Findings depend on source data, definitions, filters, transformations and KPI calculations.
- Descriptive comparisons do not establish the causes of repayment outcomes.
- Validate common identifiers before relating datasets.
- Do not publish personal, confidential, identifiable or restricted financial information.
- Confirm redistribution rights for source workbooks, PBIX and third-party materials before making the repository public.

## Future Enhancements

- Add verified data-quality statistics.
- Document the final Power BI model and relationships.
- Include exact DAX measure definitions.
- Add sanitized dashboard screenshots.
- Include validated business insights and recommendations.
- Add a data refresh guide.

## Author

**Vamshi Sabbani**  
Data Analytics Portfolio Project

## License

Include a license only for materials you have rights to share. A license for original work does not grant permission to redistribute third-party datasets or confidential materials.
