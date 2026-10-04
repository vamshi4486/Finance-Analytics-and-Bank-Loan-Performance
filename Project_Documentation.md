# Project Documentation: Finance Analytics & Bank Loan Performance

## 1. Project Summary
This project explores customer bank-loan and financial data using Microsoft Power BI and two Excel source workbooks, `Finance_1.xlsx` and `Finance_2.xlsx`. The project presentation describes each workbook as containing more than 39,000 records.

## 2. Problem Statement
Financial loan datasets contain large volumes of information about loan amounts, borrower attributes, credit history, verification status, loan status and repayment activity. When records are maintained across multiple Excel workbooks, it can be difficult to review the data consistently and understand how loan portfolio measures vary across time, geography and customer segments.

This project addresses the need for a consolidated, interactive analytical view of the bank-loan data. Microsoft Power BI is used to organize relevant loan and repayment attributes into report visuals and KPI areas, allowing users to explore year-wise loan amounts, revolving balances by grade and sub-grade, payment totals by verification status, loan status by state and month, and last payment dates across home ownership categories. The report supports descriptive analysis and exploration, not credit scoring or automated lending decisions.

## 3. Project Objectives
- Analyze year-wise loan amount statistics.
- Explore revolving balances across loan grades and sub-grades.
- Compare total payments for verified and non-verified statuses.
- Analyze loan status across states and months.
- Explore home ownership categories in relation to last payment dates.

## 4. Data Sources
- `Finance_1.xlsx`: loan details, borrower attributes, loan grades, verification status, loan status and geographic information.
- `Finance_2.xlsx`: credit history, revolving balances, repayment details, outstanding principal and payment dates.

Both observed workbook headers contain `id`. Validate uniqueness, missing values and matching records before using it as a relationship key.

## 5. KPI and Visual Analysis Requirements
| KPI area | Description |
|---|---|
| Year-wise loan amount statistics | Analyze loan amounts by year |
| Grade/sub-grade-wise revolving balance | Explore revolving balances across loan grades |
| Verified vs. non-verified total payment | Compare payment totals by verification group |
| State-wise and month-wise loan status | Explore status across geography and time |
| Home ownership vs. last payment date | Compare last payment date patterns by home ownership |

Confirm exact measures, date fields, filters and visual types in the final PBIX before documenting them as implemented.

## 6. Suggested Analytical Workflow
1. Inspect workbook structure, field names, data types and record counts.
2. Check missing values, duplicates, date formats and numeric ranges.
3. Validate `id` uniqueness and matching records across workbooks.
4. Load approved data into Power BI and configure relationships based on validated keys.
5. Prepare measures and visualizations for the specified KPI areas.
6. Validate totals, filters, slicers and report interactions.
7. Capture sanitized screenshots and document verified findings.

This is a suggested workflow; retain only the steps actually performed in the project.

## 7. Report Contents
The Power BI report is included as `PowerBI/Finance_Project.pbix`. Open it in Power BI Desktop to inspect actual report pages, visuals, relationships and measures.

## 8. Limitations and Responsible Use
- Analysis is descriptive and does not establish causes of repayment outcomes.
- Results depend on data definitions, filters, transformations and measure logic.
- Validate common identifiers before joining or relating data.
- Do not publish borrower-identifiable, confidential or restricted financial information.
- Confirm redistribution rights for source workbooks and report assets before public release.

## 9. Future Enhancements
- Add verified data-quality statistics.
- Document the final semantic model and relationships.
- Add exact DAX measure definitions.
- Include sanitized dashboard screenshots and validated business findings.
