# Marketing Analytics for a Food Delivery Platform
_Udacity Data Analyst Nanodegree - Project 5 - Data Visualization_

## Project Overview
This project has two parts that demonstrate the importance and value of data visualization techniques in the data analysis process.

1. In Part I, **Exploratory** data visualization, you will use Python visualization libraries to systematically explore a selected dataset, starting from plots of single variables and building up to plots of multiple variables.
2. In Part II, **Explanatory** data visualization, you will produce a short presentation that illustrates interesting properties, trends, and relationships that you discovered in your selected dataset. The primary method of conveying your findings will be through transforming your exploratory visualizations from the first part into polished, explanatory visualizations.

## Why this project?
Data visualization is an important skill that is used in many parts of the data analysis process.

- **Exploratory** data visualization generally occurs during and after the data wrangling process, and is the main method that you will use to understand the patterns and relationships present in your data. This understanding will help you approach any statistical analyses and will help you build conclusions and findings. This process might also illuminate additional data cleaning tasks to be performed.
- **Explanatory** data visualization techniques are used after generating your findings, and are used to help communicate your results to others. Understanding design considerations will make sure that your message is clear and effective. In addition to being a good producer of visualizations, going through this project will also help you be a good consumer of visualizations that are presented to you by others.


## Dataset

#### Content

The dataset `marketing_data.csv` was downloaded from a [kaggle dataset](https://www.kaggle.com/jackdaoud/marketing-data) and consists of 2,240 customers of a online food ordering and food delivery platform. The dataset contains data on:
- Customer profiles
- Product preferences
- Campaign successes/failures
- Channel performance

#### Acknowledgement

Credit to Dr. Omar Romero-Hernandez for providing this data set for his students. And credit to Jack Daoud for uploading and maintaining this data on Kaggle.

#### Data wrangling

The following issues where identfied and rectified accordingly:
1. Dataframe columns are sorted unintuitively
2. ` Income ` column has unnecessary leading and trailing spaces and `Year_Birth`, `Complain`, `Recency`, and `Dt_Customer` are unnatural
3. ` Income` is not formatted correctly (contains dollar signs and commas
4. `Education` values are ambiguous 
5. `Marital_Status` values are ambiguous
6. `Country` values are ambiguous
7. ` Income ` contains null values (2016 verses 2040 of the other columns
8. ` Income `, `dt.customer`, `Education`, `Marital_Status`, and `Country` have incorrect dtypes
9. `Year_Birth` has a low values under 1930 that are likely misentries


## Summary of Findings

After cleaning this dataset, it contains 2233 unique customer IDs and 28 variables. These variables detail the customers' profiles, purchasing habits, campaign successes/failures, and other marketing metrics. Most variables are either numerical or categorical in nature.
I'll be looking for correlations and relationships between numerical and categorical variables. In my main notebook, I divided my exploratory visualization into three sections:

Section 1: Univariate Exploration (6.1)\
Section 2: Bivariate Exploration (6.2)\
Section 3: Multivariate Exploration (6.3)

- There was a strong positive relationship between income and educational level.
- Wine was the most popular product, amounting to over 50% of sales. 
- Doctorates particularly enjoy wine. Doctorates from Germany especially. 
- Out of the 7 countries survey, a huge majority come from Spain, which perhaps accounts for popularity of wine and meat.
- Surprisingly, those with 0 dependents had the highest income, and therefore spent the most and made the most purchases.
- Unsurprisingly, those with only high school education made fewer purchases and spent less in general.
- The most recent campaign was the most successful while #2 campaign was least successful.
- Most customers still preferred shopping in-store rather than using catalogs.

## Key Insights for Slide-Deck Presentation

There were many threads to explore but I'll be looking mainly at these topics. The number on the bulleted lists represent the title and order of the visualizations used as they appeared in the exploratory section.

1. Campaign success
    - #14 Number of campaign success and success rate (horizontal bar plots)>
    - #25 Relationship between campaign success rate and country (facetted horizontal barplots)
2. Sales channel
    - #11 Number of purchases by sales channel (histograms)
    - #12 Share of purchases by sales channel (horizontal barplot)
    - #13 Average number of purchases per channel per ID (horizontal bar plot)
3. Purchasing trends
    - #8 Average amount spent per product per customer (horizontal barplot)
    - #9 Share of spending by product type (horizontal barplot)
4.  Number of dependents
    - #10 Number of dependents per household (barplots)
    - #21 Correlation between numerical variables (heat map)
    - #22 Income, total amount spent, and total purchases vs number of dependents (regression plots)
    - #32 Relationship between income, total amount spent, and the number of dependents (categorical scatter plot)

