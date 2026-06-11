# A/B Testing Analysis on Marketing Ad Campaign Performance

## Project Overview

This project analyzed the performance of a digital marketing advertising campaign using A/B testing.  
The goal was to evaluate whether users exposed to the advertisement showed a statistically significant improvement in conversion rate compared with the control group.
The analysis used 600K+ user-level records to examine traffic patterns, ad exposure frequency, conversion behavior, and peak conversion windows.

---

## Business Objective

The main objective of this project was to answer:
- Did the advertising campaign significantly improve user conversion?
- When were users most likely to convert?
- Were there low-efficiency ad exposure periods?
- How could ad scheduling be optimized to improve marketing ROI?

---

## Dataset

The dataset contains user-level marketing campaign records, including:

- User ID
- Test group assignment: ad group vs. control group
- Conversion outcome
- Number of ads shown
- Day of week
- Hour of day

Dataset size:

- 600K+ user records
- Treatment group: users exposed to ads
- Control group: users exposed to PSA/control content

---

## Methodology

### 1. Exploratory Data Analysis

Analyzed campaign performance across:

- Conversion rate by group
- Ad exposure frequency
- Conversion patterns by day of week
- Conversion patterns by hour of day
- Most Ads Seen by Day of the Week
- Top 10 Most Ads Seen by Day and Hour - Treatment vs. Control

### 2. A/B Hypothesis Testing

Conducted statistical tests to evaluate campaign effectiveness:

- Two-sample t-test for conversion rate difference
- Mann-Whitney U test for ad exposure frequency comparison

Hypotheses:

- Null Hypothesis: There is no significant difference in conversion rate between the ad group and the control group.
- Alternative Hypothesis: The ad group has a significantly different conversion rate from the control group.

---

## Key Findings

### 1. Ad Campaign Improved Conversion Rate

The ad group achieved a higher conversion rate than the control group:

| Group | Conversion Rate |
|---|---:|
| Ad Group | 2.55% |
| Control Group | 1.79% |

The difference was statistically significant with p-value < 0.05.

### 2. Peak Conversion Windows Identified

The analysis identified specific time periods with stronger conversion performance.  
These high-conversion windows can be prioritized for future ad scheduling.

### 3. Low-Efficiency Ad Slots Detected

Some ad delivery periods showed relatively low conversion efficiency.  
Reducing spend during these periods may help improve campaign ROI.

---

## Business Recommendations

Based on the analysis, I recommend:

- Reallocating ad budget toward high-conversion time windows
- Reducing ad delivery during low-efficiency periods
- Monitoring ad exposure frequency to avoid inefficient impressions
- Using A/B testing results to support future campaign launch decisions

---

## Tools Used

- SQL
- Python
- pandas
- matplotlib / seaborn
