# Marketing A/B Test

## 📌 Project Overview
This project analyzes a marketing A/B testing dataset to evaluate a business claim:

> **"Users who saw the most ads on Saturday converted more than users exposed on other days."**

Using statistical hypothesis testing, we compare conversion rates between users whose highest ad exposure occurred on **Saturday** versus users exposed on **other weekdays**.
---
## 🎯 Objectives
- Perform exploratory data analysis (EDA)
- Compute conversion rates for Saturday vs other days
- Test the marketing claim using a **Two-Proportion Z-Test**
- Calculate **95% Confidence Intervals** for conversion rates
- Provide actionable business insights based on statistical results
---
## ⭐ Key Takeaways
- Compared conversion rates between **Saturday vs other weekdays** using hypothesis testing  
- Applied a **One-sided Two-Proportion Z-Test** to evaluate a marketing claim  
- Computed **95% Confidence Intervals (Wilson method)** for conversion rate estimates  
- Found that Saturday conversion rate was **significantly lower** than other days  
- Delivered business recommendations based on statistical evidence

---
## 📊 Key Metric

- `converted = True` means the user completed the desired action (conversion)
- `converted = False` means the user did not convert

---
## 🧪 Hypothesis Testing
We compare two groups:

- **Saturday group:** users where `most ads day = Saturday`
- **Other days group:** users where `most ads day ≠ Saturday`

Null Hypothesis (H0)
Alternative Hypothesis (H1)
This is a **one-sided hypothesis test**, based on the business claim that Saturday performs better.

---
## 📈 Results Summary

| Group        | Users   | Converted | Conversion Rate | 95% CI Lower | 95% CI Upper |
|-------------|---------|-----------|----------------|--------------|--------------|
| Saturday     | 81,660  | 1,719     | 2.11%          | 2.01%        | 2.21%        |
| Other days   | 506,441 | 13,124    | 2.59%          | 2.55%        | 2.64%        |

### Two-Proportion Z-Test Output
- **Z-statistic:** -8.223  
- **P-value (one-sided):** 1.00000  

---
## 🧠 Interpretation
The conversion rate for Saturday users is **lower** than the conversion rate for users exposed on other days.

The confidence intervals do not overlap, indicating that the difference is robust and unlikely to be explained by random sampling variation.

---
## ✅ Conclusion
The statistical results do **not support** the marketing claim that Saturday generates higher conversions.

Since the p-value is far above 0.05, we **fail to reject the null hypothesis**.  
In fact, the observed results suggest that Saturday performs **worse** than other days in terms of conversion rate.

---
## 💡 Business Recommendation
Based on the data:

- Increasing ad budget on Saturdays is **not recommended** without further investigation.
- Marketing teams may benefit from reallocating spend to higher-performing weekdays.
- Future analysis should explore segmentation by:
  - `test group` (ad vs psa)
  - `total ads` exposure level
  - `most ads hour`

---
## 🛠 Tools & Libraries
- Python 3
- pandas
- numpy
- matplotlib
- statsmodels
---
## 🚀 Future Improvements
- Weekend vs Weekday analysis (Saturday + Sunday vs Monday–Friday)
- Logistic regression model for conversion prediction
- Segment-level hypothesis testing by ad exposure intensity
- Multiple comparisons correction when testing multiple weekdays

---
## 👤 Author
Created by: zohreh samieekadkani LinkedIn:https://www.linkedin.com/in/zohrehsamiee/
