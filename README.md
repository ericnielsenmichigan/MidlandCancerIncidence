
# Michigan Cancer Incidence & Industrial Carcinogen Analysis
An exploratory data analysis investigating whether industrial carcinogen releases correlate with county-level cancer incidence across Michigan, with a focused case study on Midland County and the Dow Chemical plant.
Overview
Using EPA Toxic Release Inventory (2005) data merged with the Michigan Cancer Data Atlas (2015–2019), this analysis examines two questions:

Do Michigan counties with higher carcinogen releases have higher cancer rates, after controlling for smoking, obesity, poverty, and race?
Is Midland County's cancer incidence significantly elevated compared to demographically similar counties?

Key Findings

No meaningful county-level relationship between carcinogen release and cancer incidence (Pearson r = 0.045, p = 0.68)
Obesity, poverty, and smoking are the strongest predictors of cancer incidence at the county level
Midland County's cancer rate (463.3 per 100k) is statistically significantly higher than demographically similar counties (mean: 437.0, p = 0.037), a finding that strengthened with a larger comparison group (p < 0.001)
Midland's elevated incidence is unlikely explained by socioeconomic or demographic factors alone, warranting further investigation

Data Sources

EPA Toxic Release Inventory (TRI), 2005
Michigan Cancer Data Atlas, MDHHS, 2015–2019
U.S. Census Bureau, 2020 Decennial Census

Methods

Log transformation of skewed carcinogen release data
Pearson correlation and multivariate linear regression (5 predictors, 83 county observations)
One-sample t-test comparing Midland County to matched comparison groups (2% and 4% similarity windows on poverty rate and % non-white)

Tools
Python, Pandas, Matplotlib
