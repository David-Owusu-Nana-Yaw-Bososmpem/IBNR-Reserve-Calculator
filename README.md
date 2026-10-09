# IBNR Reserve Calculator & Reserving Model

## Overview

This project is an Excel-based actuarial reserving model developed to estimate **Ultimate Claims** and **Incurred But Not Reported (IBNR) reserves** using reported claims and completion factors.

The model uses six months of reported claims data and applies completion factors based on company size and claim type to estimate outstanding claim liabilities.

## Project Objectives

The model was developed to:

- Estimate ultimate claims from reported claims data
- Calculate IBNR reserves using completion factors
- Classify companies according to employee count
- Apply claim-specific and company-size-specific completion factors
- Provide a structured Excel-based reserving workflow
- Reduce the time required to perform reserve calculations

## Reserving Methodology

The model estimates ultimate claims by applying completion factors to reported claims.

The general reserving relationship is:

**IBNR Reserve = Estimated Ultimate Claims − Reported Claims**

Completion factors vary according to:

- Company size
- Claim type
- Claim development period

This allows the model to account for differences in claim reporting and development patterns.

## Company Size Classification

Companies are classified into three categories according to employee count:

- **Small:** 1–100 employees
- **Medium:** 101–5,000 employees
- **Large:** 5,001+ employees

The appropriate company-size classification is combined with the selected claim type to determine the applicable completion factors.

## Claim Types

The model incorporates three claim categories:

- Dental
- Prescription
- Healthcare Appointment

Each combination of company size and claim type has its own set of monthly completion factors.

## Model Inputs

The calculator uses:

- Employee count
- Claim type
- Monthly reported claims
- Completion factors

Reported claims cover a six-month period from **January 2020 through June 2020**.

## Model Outputs

The model calculates:

- Company size category
- Applicable completion factors
- Estimated ultimate claims
- IBNR reserve

The resulting reserve represents the estimated portion of ultimate claims that has not yet been reported.

## Workbook Structure

The Excel workbook contains five main worksheets:

### Calculator

The main calculation interface used to:

- Enter or reference employee count
- Select a claim type
- Review monthly reported claims
- Retrieve applicable completion factors
- Estimate ultimate claims
- Calculate the IBNR reserve

### Company_Data

Contains company-level information including:

- Company identifier
- Company type
- Company size
- Monthly reported claims
- IBNR reserve information

### Completion_Factors

Contains completion factors segmented by:

- Company size
- Claim type
- Development month

These factors are referenced by the calculator when estimating ultimate claims.

### Reported_Claims

Contains example reported claims data for the six-month development period, together with employee counts and claim types.

### Pivot_Table

Summarizes company and claims information to support analysis of the underlying data.

## Excel Functionality

The workbook uses Excel functionality including:

- Lookup formulas
- Conditional logic
- Dynamic cell references
- Completion-factor calculations
- PivotTables
- Structured reserving calculations

For example, the calculator automatically determines the company-size category from employee count and retrieves the corresponding completion factors for the selected claim type.

## Repository Structure

```text
IBNR-Reserve-Calculator/
│
├── IBNR_Reserve_Calculator.xlsm
└── README.md
```

## Skills Demonstrated

- Actuarial reserving
- IBNR estimation
- Ultimate claims estimation
- Completion-factor methodology
- Claims analysis
- Insurance liability estimation
- Microsoft Excel
- Lookup and conditional formulas
- PivotTables
- Actuarial model development

## Author

**David Nana Yaw Owusu Bosompem**

BSc Actuarial Science  
SOA Exam P & FM

**Interests:** Actuarial Science | Insurance Analytics | Predictive Modeling | Statistics
