# Marketing Campaign Analysis: Facebook Ads vs Google AdWords

## About the Project

In digital marketing, simply getting more clicks doesn't always mean getting better results. This project compares the performance of two advertising platforms—Facebook Ads and Google AdWords—to understand which one is more effective at generating conversions and delivering better value for advertising spend.

Using campaign data from 2019, I analyzed daily metrics such as views, clicks, conversions, CTR, CPC, and advertising costs to identify trends and evaluate overall campaign performance.

---

## Objective

The main goal of this analysis is to answer the following question:

> Which platform performs better in terms of conversions, engagement, and cost-effectiveness: Facebook Ads or Google AdWords?

The insights from this analysis can help marketers make better decisions about budget allocation and campaign optimization.

---

## Dataset

The dataset contains daily advertising performance data for both Facebook and Google AdWords campaigns throughout 2019.

### Features Included

- Date
- Ad Views
- Ad Clicks
- Ad Conversions
- Ad Cost
- Click Through Rate (CTR)
- Conversion Rate
- Cost Per Click (CPC)

Total records: **365 days of campaign data**

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-Learn
- Statsmodels

---

## Analysis Performed

### Data Cleaning

- Converted date columns into datetime format
- Removed currency symbols and percentage signs
- Converted metrics into numerical values for analysis

### Exploratory Data Analysis

- Distribution of clicks and conversions
- Campaign performance comparison
- Conversion frequency analysis
- Monthly and weekly trends

### Correlation Analysis

I analyzed whether increasing ad clicks actually leads to more conversions.

**Results:**

| Platform | Correlation |
|-----------|------------|
| Facebook | 0.87 |
| AdWords | 0.45 |

Facebook showed a much stronger relationship between clicks and conversions.

---

### Hypothesis Testing

To verify whether Facebook actually performs better than AdWords, I conducted an independent two-sample t-test.

**Average Conversions**

- Facebook: 11.74
- AdWords: 5.98

The p-value obtained was extremely small (< 0.05), indicating a statistically significant difference between the two platforms.

**Conclusion:** Facebook generates significantly more conversions than AdWords.

---

### Regression Analysis

A Linear Regression model was built to predict Facebook conversions based on the number of clicks.

**Model Performance**

- R² Score: 76.35%
- Mean Squared Error: 2.02

Example predictions:

| Clicks | Expected Conversions |
|---------|--------------------|
| 50 | 13 |
| 80 | 19.31 |

---

### Time Series Analysis

I also examined how conversions change over time.

#### Weekly Trends

- Conversions remain relatively stable throughout the week.
- Mondays and Tuesdays tend to have slightly higher conversion counts.

#### Monthly Trends

An overall upward trend in conversions was observed, with some fluctuations during certain months.

---

### Cost Per Conversion Analysis

Cost Per Conversion was analyzed to identify the most cost-effective periods for advertising.

**Key Findings**

- Lowest CPC: May and November
- Highest CPC: February

This suggests that campaigns run during certain months may provide better ROI.

---

### Cointegration Analysis

To understand the long-term relationship between advertising spend and conversions, a cointegration test was performed.

The results showed a significant long-term relationship between campaign cost and conversions, indicating that advertising spend has a measurable impact on campaign outcomes over time.

---

## Key Findings

- Facebook consistently generated more conversions than AdWords.
- Facebook clicks were much more likely to turn into conversions.
- AdWords received more clicks on average but converted less effectively.
- Certain months provided better cost efficiency than others.
- Advertising spend and conversions show a strong long-term relationship.

---

## Final Conclusion

Based on the analysis, **Facebook Ads outperformed Google AdWords in terms of conversion generation and overall effectiveness**.

Although AdWords attracted more clicks, Facebook was significantly better at turning those clicks into actual conversions. The statistical tests, correlation analysis, and predictive modeling all support this conclusion.

For businesses focused on maximizing conversions and improving ROI, Facebook appears to be the stronger advertising platform based on this dataset.

---

