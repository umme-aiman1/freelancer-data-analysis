# Freelancer Data Analysis

## Project Overview

This project analyzes a dataset of 1,000 freelancers to understand patterns in freelancer demographics, professional experience, hourly rates, ratings, client satisfaction, skills, countries, and activity status.

The project follows a complete data analysis workflow including data cleaning, exploratory data analysis, statistical analysis, and data visualization using Python.

## Objectives

- Analyze freelancer demographics and experience.
- Identify common freelancer skills.
- Compare hourly rates across countries.
- Analyze the relationship between experience and hourly rates.
- Analyze the relationship between ratings and hourly rates.
- Compare active and inactive freelancers.
- Analyze client satisfaction.
- Explore correlations between numerical variables.
- Present findings using data visualizations.

## Dataset

The dataset contains **1,000 freelancer records**.

### Main Features

- `freelancer_id` – Unique freelancer identifier
- `name` – Freelancer name
- `gender` – Gender
- `age` – Freelancer age
- `country` – Country
- `language` – Primary language
- `primary_skill` – Main professional skill
- `years_of_experience` – Years of professional experience
- `hourly_rate_usd` – Hourly rate in USD
- `rating` – Freelancer rating
- `is_active` – Active/inactive status
- `client_satisfaction` – Client satisfaction score

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning

The dataset was cleaned before performing the analysis.

The following steps were performed:

- Handled missing numerical values using median imputation.
- Handled missing `is_active` values using the mode.
- Checked for duplicate rows.
- Checked data types.
- Checked for invalid ages.
- Checked for negative experience values.
- Checked for negative hourly rates.
- Checked ratings outside the 0–5 range.
- Checked client satisfaction values outside the 0–100 range.

### Validation Results

- Missing values after cleaning: **0**
- Duplicate rows: **0**
- Invalid ages: **0**
- Negative experience values: **0**
- Negative hourly rates: **0**
- Invalid ratings: **0**
- Invalid satisfaction values: **0**

## Exploratory Data Analysis

The following analyses were performed:

### Freelancer Overview

- Average age: **40.52 years**
- Average experience: **11.22 years**
- Average hourly rate: **$51.29**
- Average rating: **2.52 / 5**
- Average client satisfaction: **79.22 / 100**
- Active freelancers: **63.2%**

### Experience vs Hourly Rate

The correlation between years of experience and hourly rate was **0.08**, indicating a very weak linear relationship.

### Age vs Experience

Age and years of experience had a correlation of **0.60**, indicating a moderate positive relationship.

### Rating vs Hourly Rate

The correlation between rating and hourly rate was **0.02**, showing almost no linear relationship.

### Active vs Inactive Freelancers

| Metric | Inactive | Active |
|---|---:|---:|
| Hourly Rate | $50.75 | $51.61 |
| Rating | 2.47 | 2.55 |
| Client Satisfaction | 79.27 | 79.19 |
| Experience | 10.84 years | 11.44 years |

## Visualizations

The project includes the following visualizations:

- Average Hourly Rate by Years of Experience
- Top 10 Countries by Average Hourly Rate
- Average Hourly Rate by Freelancer Rating
- Active vs Inactive Freelancers
- Correlation Heatmap

## Key Findings

- The dataset contains 1,000 freelancers.
- The average freelancer is approximately 40.5 years old.
- The average freelancer has approximately 11.2 years of experience.
- The average hourly rate is approximately $51.29.
- 63.2% of freelancers are active.
- Active freelancers have a slightly higher average hourly rate and rating than inactive freelancers.
- Experience has a very weak relationship with hourly rate.
- Age and experience have a moderate positive relationship.
- Rating and hourly rate have almost no linear relationship.
- Rating and client satisfaction also have almost no linear relationship.

## Project Structure

```text
Freelancer-Data-Analysis/
│
├── data/
│   └── freelancer_data.csv
│
├── notebooks/
│   └── data_cleaning.ipynb
│
├── report/
│   ├── Freelancer_Data_Analysis_Project_Report.docx
│   ├── experience_vs_hourly_rate.png
│   ├── hourly_rate_by_country.png
│   ├── rating_vs_hourly_rate.png
│   ├── active_vs_inactive.png
│   └── correlation_heatmap.png
│
└── screenshots/
    ├── 01_project_overview.png
    ├── 02_data_cleaning_validation.png
    ├── 03_basic_statistics.png
    ├── 04_top_countries.png
    ├── 05_top_skills.png
    ├── 06_active_vs_inactive.png
    ├── 07_experience_vs_hourly_rate.png
    ├── 08_hourly_rate_by_country.png
    ├── 09_rating_vs_hourly_rate.png
    ├── 10_active_vs_inactive_chart.png
    ├── 11_correlation_heatmap.png
    └── 12_key_insights_conclusion.png
