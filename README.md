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

- The dataset contained **516 records initially**. After removing
  duplicate customer records using the documented most-recent-record
  rule, **500 unique customer records** remained.
- Missing regional information was a notable data-quality issue, with
  **60 of the 500 records (12%)** having no region recorded.
- Among records with a known region, **Asia-Pacific had the highest
  proportion of incomplete records at 11.11%**, based on missing email,
  signup date or age.
- Customer sign-up activity increased noticeably from 2024 onwards,
  although the presence of invalid and future dates means trends should
  be interpreted with caution.
- **August 2026** was the latest valid month with recorded signup
  activity. Google generated the signup recorded during that month.
  However, because only one signup was recorded, this result should not
  be interpreted as evidence that Google was the best-performing
  acquisition channel overall.
- Marketing opt-in rates varied across age groups. The **18–24 group
  had the highest opt-in rate at 68.42%**, while the **45–54 group had
  the lowest at 30.00%** among the analysed age groups.
- **Basic** was the most commonly selected plan overall, accounting for
  **48% of customers**, followed by Pro at 36.8% and Premium at 15.2%.
  Plan preferences also varied across age groups.

## Business Recommendations

- Improve data validation at the point of customer entry, particularly
  for email addresses, ages, signup dates and regional information.
- Strengthen duplicate-prevention controls so that repeated customer
  records are identified before they enter reporting datasets.
- Investigate the causes of missing regional information and improve
  the collection of this field, as missing region data can affect
  regional campaign and customer analysis.
- Monitor acquisition sources over several complete reporting periods
  before making investment decisions, using additional measures such as
  conversion, acquisition cost and customer value rather than signup
  volume alone.
- Consider age-specific marketing approaches, particularly when
  evaluating differences in marketing opt-in behaviour across customer
  segments.
- Further investigate plan preferences across age groups to determine
  whether different customer segments respond differently to Basic,
  Pro and Premium offerings.

## Data Limitations

The analysis considers the limitations associated with missing,
invalid and potentially anomalous records.

In particular:

- Two signup dates could not be used for time-based analysis because
  they were invalid.
- Future signup dates were identified and flagged rather than deleted,
  as their validity could not be established from the available data.
- Five implausible age values were treated as missing because there was
  insufficient information to determine their correct values.
- Missing regional information was retained where it could not be
  reliably inferred.
- The latest valid month contained only one recorded signup, so the
  acquisition-source finding for that period has limited significance.
- The dataset provides descriptive insights but does not establish
  causal relationships between customer characteristics and behaviour.

## Project Files

- `notebooks/` – Analysis notebook
- `data/` – Project dataset, where appropriate for public sharing
- `visualisations/` – Key charts
- `reports/` – Final analytical report

## Author

**Mujeeb Sonibare**

GitHub: [mujeebsonibare](https://github.com/mujeebsonibare)
