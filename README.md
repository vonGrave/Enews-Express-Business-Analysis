# E-news Express A/B Testing Analysis

## Project Overview
This project analyzes the results of an A/B test conducted by E-news Express, comparing the effectiveness of a new landing page design against their existing page. The analysis focuses on user engagement metrics and conversion rates across different language preferences.

## Dataset Description
The dataset (Enews_data.csv) contains 100 records with the following features:
- user_id: Unique identifier for each user
- group: Test group (control/treatment)
- landing_page: Page version shown (old/new)
- time_spent_on_the_page: Time spent by user (in minutes)
- converted: Whether the user subscribed (yes/no)
- language_preferred: User's preferred language (English/French/Spanish)

## Analysis Performed
1. Comparison of time spent on old vs new pages
2. Analysis of conversion rates between page versions
3. Statistical testing of language preference impact on:
- Conversion rates (Chi-square test)
- Time spent on page (One-way ANOVA)

## Key Findings
1. Users spend significantly more time on the new page design
2. The new page shows higher conversion rates compared to the old version
3. Conversion rates are independent of language preference
4. Time spent on the new page is consistent across all language preferences

## Recommendations
Based on the analysis, it is recommended that E-news Express:
- Implement the new landing page design
- Maintain the current multi-language support strategy
- Continue monitoring engagement metrics across different user segments

## Technical Details
Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scipy.stats

## Statistical Tests Applied
- Shapiro-Wilk test (normality)
- Levene's test (variance homogeneity)
- One-way ANOVA
- Chi-square test

## Running the Analysis
The analysis is contained in a Jupyter notebook (Business_Statistics_Enews_Express.ipynb). To run the analysis:

1. Ensure all required libraries are installed
2. Place the Enews_data.csv file in the same directory as the notebook
3. Run all cells in the notebook sequentially
