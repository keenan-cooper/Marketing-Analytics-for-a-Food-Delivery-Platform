# Marketing Analytics for a Food Delivery Platform
## by Keenan Cooper


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
| 1 |Dataframe columns are sorted unintuitively|
| 2 |` Income ` column has unnecessary leading and trailing spaces and `Year_Birth`, `Complain`, `Recency`, and `Dt_Customer` are unnatural
| 3 |` Income` is not formatted correctly (contains dollar signs and commas|
| 4 |`Education` values are ambiguous |
| 5 |`Marital_Status` values are ambiguous|
| 6 |`Country` values are ambiguous|
| 7 |` Income ` contains null values (2016 verses 2040 of the other columns|
| 8 |` Income `, `dt.customer`, `Education`, `Marital_Status`, and `Country` have incorrect dtypes|
| 9 |`Year_Birth` has a low values under 1930 that are likely misentries|


## Summary of Findings

After cleaning this dataset, it contains 2233 unique customer IDs and 28 variables. These variables detail the customers' profiles, purchasing habits, campaign successes/failures, and other marketing metrics. Most variables are either numerical or categorical in nature.
I'll be looking for correlations and relationships between numerical and categorical variables. In my main notebook, I divided my exploratory visualization into three sections. The titles of the visualizations should make it clear what I was looking for and how I went about investigating the data.

Section 1: Univariate Exploration (6.1)
1. Number of registrations per year (barplot)
2. Distribution of income (histogram)
3. Distribution of birth year (histogram)
4. Distribution of ages (boxplot)
5. Number of IDs by education, marital status, and country (categorical barplot)
6. Distribution of spending by product type (histograms)
7. Distribution of total spending (histogram)
8. Average amount spent per product per customer (horizontal barplot)
9. Share of spending by product type (horizontal barplot)
10. Number of dependents per household (barplots)
11. Number of purchases by sales channel (histograms)
12. Share of purchases by sales channel (horizontal barplot)
13. Average number of purchases per channel per ID (horizontal bar plot)
14. Number of campaign success and success rate (horizontal bar plots)

Section 2: Bivariate Exploration (6.2)
15. Income distribution by country, education level, and marital status (facetted histograms)
16. Mean income by country, education level, and marital status (categorical bar charts)
17. Total number purchases by country, education level, and marital status (categorical bar charts)
18. Mean number of purchases by country, education level, marital status (categorical bar charts)
19. Distribution of amount spent and number of purchases vs categorical variables (violin plots)
20. Distribution of amount spent by product type against number of dependents (boxplots)
21. Correlation between numerical variables (heat map)
22. Income, total amount spent, and total purchases vs number of dependents (regression plots) (regression plots)
23. Relationship between country and education level (heat map)
24. Relationship between country and marital status (countplot)
25. Relationship between campaign success and country (facetted horizontal barplots)

Section 3: Multivariate Exploration (6.3)
26. Relationship between number of purchases, education, and number of dependents (clustered boxplots)
27. Relationship between total amount purchased, country, and marital status (clustered boxplots)
28. Relationship between amount spent on wine, country, education (categorical boxplots)
29. Relationship between mean amount spent on gold, marital status, and the number of dependents (categorical barplot)
30. Relationship between the total amount spent on gold, country, and the number of dependents (categorical split plot)
31. Relationship between the total amount spent on gold, education, and the number of dependents (categorical point plot)
32. Relationship between income, total amount spent, and the number of dependents (categorical scatter plot)
33. Relationship between education, marital status, total amount spent, and the number of purchases (facetted scatter plots)

- There was a strong positive relationship between income and educational level.
- Wine was the most popular product, amounting to over 50% of sales. 
- Doctorates particularly enjoy wine. Doctorates from Germany especially. 
- Out of the 7 countries survey, a huge majority come from Spain, which perhaps accounts for popularity of wine and meat.
- Surprisingly, those with 0 dependents had the highest income, and therefore spent the most and made the most purchases.
- Unsurprisingly, those with only high school education made fewer purchases and spent less in general.
- The most recent campaign was the most successful while #2 campaign was least successful.
- Most customers still preferred shopping in-store rather than using catalogs.

## Key Insights for Presentation

There were many threads to explore but I'll be looking mainly at these topics:

1. Campaign success
    14. Number of campaign success and success rate (horizontal bar plots)
    25. Relationship between campaign success rate and country (facetted horizontal barplots)
2. Sales channel
    11. Number of purchases by sales channel (histograms)
    12. Share of purchases by sales channel (horizontal barplot)
    13. Average number of purchases per channel per ID (horizontal bar plot)
3. Purchasing trends
    8. Average amount spent per product per customer (horizontal barplot)
    9. Share of spending by product type (horizontal barplot)
4.  Number of dependents
    10. Number of dependents per household (barplots)
    21. Correlation between numerical variables (heat map)
    22. Income, total amount spent, and total purchases vs number of dependents (regression plots)
    32. Relationship between income, total amount spent, and the number of dependents (categorical scatter plot)

