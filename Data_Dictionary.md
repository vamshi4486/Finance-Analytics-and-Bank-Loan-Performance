# Data Dictionary: Finance Loan Analysis

This dictionary records source fields observed in the uploaded workbook headers. Confirm exact business definitions, units and allowed values against the source specification and Power BI model.

## Finance_1.xlsx – Loan and Borrower Attributes

| Field | Description |
|---|---|
| `id` | Loan or record identifier |
| `member_id` | Source member identifier; treat as sensitive |
| `loan_amnt` | Loan amount |
| `funded_amnt` | Funded amount |
| `funded_amnt_inv` | Amount funded by investors |
| `term` | Loan term |
| `int_rate` | Interest rate |
| `installment` | Installment amount |
| `grade` | Loan grade |
| `sub_grade` | Loan sub-grade |
| `emp_title` | Employment title; may be free text |
| `emp_length` | Employment length |
| `home_ownership` | Home ownership category |
| `annual_inc` | Annual income |
| `verification_status` | Verification category |
| `issue_d` | Loan issue date |
| `loan_status` | Loan status category |
| `pymnt_plan` | Payment plan indicator/category |
| `desc` | Free-text description; inspect for sensitive information |
| `purpose` | Loan purpose |
| `title` | Loan title or description |
| `zip_code` | Postal code field; review for privacy |
| `addr_state` | State or geographic category |
| `dti` | Debt-to-income ratio field |

## Finance_2.xlsx – Credit History and Repayment Attributes

| Field | Description |
|---|---|
| `id` | Loan or record identifier |
| `delinq_2yrs` | Delinquency count for source-defined two-year period |
| `earliest_cr_line` | Earliest credit-line date |
| `inq_last_6mths` | Credit inquiries in preceding six months, per source definition |
| `mths_since_last_delinq` | Months since last delinquency |
| `mths_since_last_record` | Months since last public record |
| `open_acc` | Open account count |
| `pub_rec` | Public-record count |
| `revol_bal` | Revolving balance |
| `revol_util` | Revolving utilization |
| `total_acc` | Total account count |
| `initial_list_status` | Initial listing status |
| `out_prncp` | Outstanding principal |
| `out_prncp_inv` | Outstanding principal attributed to investors |
| `total_pymnt` | Total payment amount |
| `total_pymnt_inv` | Total payment amount attributed to investors |
| `total_rec_prncp` | Principal received |
| `total_rec_int` | Interest received |
| `total_rec_late_fee` | Late fees received |
| `recoveries` | Recovery amount |
| `collection_recovery_fee` | Collection recovery fee |
| `last_pymnt_d` | Last payment date |
| `last_pymnt_amnt` | Last payment amount |
| `next_pymnt_d` | Next payment date |
| `last_credit_pull_d` | Last credit-pull date |

## Notes
- Both workbook headers contain `id`; validate key uniqueness, missing values and matches before relating the tables.
- Review nulls and blank values and document how they are handled.
- Descriptions are inferred from field names; confirm units and formal definitions before making business claims.
