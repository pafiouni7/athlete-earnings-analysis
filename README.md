# Athlete Earnings Trends (1990–2020)

## Overview
This project analyzes trends in top-earning professional athletes from 1990 to 2020, focusing on how earnings vary by sport, nationality, and ranking over time. The analysis emphasizes structural patterns in athlete compensation rather than tracking individual athletes longitudinally.

The goal is to understand how factors such as sport popularity, media exposure, and star athletes influence earnings distributions across decades.

---

## Data
- Source: Public athlete earnings dataset (Kaggle)
- Time period: 1990–2020
- Key variables:
  - Year
  - Athlete name
  - Sport
  - Nationality
  - Earnings (USD, millions)
  - Rank

### Data Preparation
- Standardized sport naming conventions (e.g., "American Football," "NFL," and "american football")
- Excluded nationalities with fewer than 10 athletes to prevent skewed averages
- Acknowledged that the dataset represents top earners per year rather than continuous athlete-level tracking

---

## Methodology
- Cleaned and standardized earnings and categorical variables
- Aggregated earnings by year, sport, nationality, and rank
- Used average earnings instead of totals to avoid overrepresentation by countries with more athletes
- Created visualizations including:
  - Line plots of average earnings by nationality over time
  - Scatter plots of individual athlete earnings across years
  - Stacked bar charts showing sport representation among top earners
- Identified "star athletes" (athletes appearing 19 or more times) and re-analyzed sport representation with these athletes removed
- Applied regression analysis to examine the relationship between athlete rank and earnings
- Evaluated model performance using predicted versus actual earnings and R-squared values

---

## Results & Key Insights
- Athlete earnings increased substantially over time, driven by inflation and the commercialization of major sports
- Basketball, American football, and golf consistently dominated representation among top earners
- Cycling and MMA showed minimal and declining representation over the 30-year period
- Removing star athletes (e.g., Tiger Woods and Michael Jordan) demonstrated how individual athletes can significantly influence a sport’s earnings profile
- Regression results showed that athletes ranked ninth and tenth sometimes earned more than those ranked seventh and eighth, reflecting sport-specific pay structures
- The prediction model exhibited a weak positive correlation (R² ≈ 0.34), with notable outliers such as Floyd Mayweather whose earnings were not well captured

---

## Limitations
- Earnings were not adjusted for inflation
- Dataset does not capture all income sources (e.g., private endorsements)
- Data ends in 2020 and does not reflect post-COVID impacts
- Extreme outliers reduce predictive accuracy in regression modeling

---

## Tech Stack
- Languages: Python, SQL
- Libraries: pandas, matplotlib, seaborn
- Tools: Jupyter Notebook

---

## Next Steps
- Adjust earnings for inflation to improve cross-decade comparability
- Extend the dataset beyond 2020 to analyze COVID-era impacts
- Explore alternative modeling approaches to better handle extreme outliers
- Incorporate additional income sources if data becomes available

---

## Conclusion
This analysis highlights how sport popularity, sponsorships, and media exposure play a significant role in shaping athlete earnings beyond athletic performance alone. The findings emphasize the importance of accounting for data structure, outliers, and limitations when interpreting economic trends in professional sports.
