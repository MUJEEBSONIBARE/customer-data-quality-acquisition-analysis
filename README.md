# Customer Data Quality & Acquisition Analysis

## Overview

This project analyses customer sign-up data to assess data quality,
identify customer acquisition patterns and generate business-focused
recommendations.

The project demonstrates an end-to-end data analysis workflow, from
initial data-quality assessment and cleaning through to exploratory
analysis, visualisation and business recommendations.

## Business Objectives

The analysis aims to:

- Assess the completeness and consistency of customer data
- Identify duplicate and invalid records
- Analyse customer acquisition sources
- Examine customer demographics and marketing behaviour
- Identify potential data-quality risks
- Translate analytical findings into practical business recommendations

## Technologies

- Python
- Pandas
- Matplotlib
- Google Colab

## Data Quality & Cleaning

The dataset was assessed for:

- Missing values
- Duplicate customer records
- Invalid signup dates
- Inconsistent categorical values
- Malformed email addresses
- Implausible age values

The cleaning process included:

- Standardising categorical values
- Correcting unambiguous email-formatting issues
- Removing duplicate customer records using a documented rule
- Flagging future signup dates for review
- Treating invalid dates as missing for time-based analysis
- Treating implausible ages as missing rather than making unsupported assumptions
- Retaining missing regional information where it could not be reliably inferred

## Analysis

The project examines:

### Customer Signups Over Time

Weekly signup trends were analysed to identify changes in customer
acquisition activity over time.

### Acquisition Sources

Customer signups were compared across acquisition channels including
Google, Instagram, Referral, Facebook, Organic and LinkedIn.

### Regional Distribution

Customer records were analysed by region while also assessing the
impact of missing regional information.

### Marketing Opt-in Behaviour

Marketing opt-in rates were examined by gender and age group.

### Plan Preferences

Customer plan selection was analysed overall and across age groups.

## Key Findings

The final findings from the analysis will be documented here.

## Business Recommendations

The final recommendations from the analysis will be documented here.

## Data Limitations

The analysis considers the limitations associated with missing,
invalid and potentially anomalous records.

## Project Files

- `notebooks/` – Analysis notebook
- `data/` – Project dataset, where appropriate for public sharing
- `visualisations/` – Key charts
- `reports/` – Final analytical report

## Author

**Mujeeb Sonibare**

GitHub: [mujeebsonibare](https://github.com/mujeebsonibare)
