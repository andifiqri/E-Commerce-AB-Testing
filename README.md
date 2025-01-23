# E-Commerce A/B Testing

This repository contains an A/B testing analysis designed to evaluate the impact of a new landing page on user conversion rates. The analysis involves comprehensive steps, including data cleaning, exploratory data analysis (EDA), and statistical hypothesis testing.

For this project, the dataset was sourced from Kaggle (https://www.kaggle.com/datasets/putdejudomthai/ecommerce-ab-testing-2022-dataset1) and represents an A/B test conducted by an e-commerce website. The company developed a new landing page aimed at increasing the number of users who "convert," meaning users who decide to pay for the company's product. The goal of this analysis is to determine whether the company should implement the new page, retain the old page, or consider extending the experiment to gather more data before making a decision.

This project aims to provide actionable insights based on robust statistical methods to support data-driven decision-making.


# Dataset Overview
The dataset used for this analysis contains the following columns:

•	user_id: Unique identifier for each user.

•	timestamp: Date and time when the user interacted with the page.

•	group: Indicates whether the user is in the control group (control) or treatment group (treatment).

•	landing_page: Type of landing page shown to the user (old_page or new_page).

•	converted: Indicates whether the user performed the desired action (1 for converted, 0 for not converted).


# Objective
The primary goal is to determine whether introducing the new landing page significantly increases the conversion rate compared to the old landing page.
The analysis answers the following questions:

1.	Does the new landing page result in a higher conversion rate?

2.	Are the differences between the groups statistically significant?

# Data Preprocessing
Steps taken to clean the dataset:

1.	Removed misaligned records where the group and landing_page columns were inconsistent (e.g., control group paired with new_page or treatment group paired with old_page).

2.	Verified the integrity of the dataset and calculated the number of records removed during cleaning.

# Exploratory Data Analysis (EDA)
Key analyses performed:

1.	Overall Conversion Rate:

    •	Calculated the overall conversion rate across both groups.

2.	Conversion Rates by Group:

    •	Computed and visualized conversion rates for the control and treatment groups.

3.	Data Distribution:

    •	Visualized the distribution of users across the control and treatment groups.

# Statistical Analysis
The following statistical tests were conducted:

1.	Z-Test for Proportions:

    •	Compared the conversion rates of the control and treatment groups.

    •	Key metrics: Z-statistic and p-value.
2.	Standard Deviation and Standard Error:

    •	Evaluated the variability and representativeness of the sample data.

# Results and Insights
Key findings from the analysis:

1. Conversion Rate Comparison:

    •	Control group: 0.120386 (~12.04%)

    •	Treatment group: 0.118806 (~11.88%)
2. The difference in conversion rates between the groups (~0.01) is very small.
3. Hypothesis Testing:

    •	Z-statistic: 1.3130

    •	P-value: 0.1892

    •	Since the p-value > 0.05, we fail to reject the null hypothesis, indicating that the new landing page does not have a statistically significant impact on conversion rates.

# Conclusion

The analysis suggests that the new landing page does not result in a significant improvement in conversion rates compared to the old landing page. The company may consider further testing or exploring other strategies to enhance user engagement and conversions.


