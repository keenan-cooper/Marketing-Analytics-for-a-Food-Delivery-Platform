# Marketing Analytics for a Food Delivery Platform
#### [_Udacity - Data Analyst Nanodegree:_](https://www.udacity.com/course/data-analyst-nanodegree--nd002) _Project 5 - Data Visualization_
## Table of Contents

1. [Project Overview](#project)
2. [Requirements](#requirements)
3. [Project Movitivation](#motivation)
4. [Key Files](#files)
5. [Summary of Findings](#summary)
6. [Acknowledgements](#acknowledgements)

### 1. Project Overview<a id="project"></a>
This project has two parts to demonstrate the importance and data visualization techniques in the data analysis process.

- Part 1: **Exploratory** data visualization\
    I used Python visualization libraries to systematically explore a dataset, starting from plots of single variables and building up to plots of multiple variables.
- Part 2: **Explanatory** data visualization\
    I produced a short presentation to illustrate interesting properties, trends, and relationships discovered in my dataset. The primary method of conveying my findings was through transforming the exploratory visualizations from part 1 into polished explanatory visualizations.

### 2. Requirements<a id="requirements"></a>
This project was created in a Jupyter Notebook made available via Anaconda and written in python. 
The following versions of languages and libraries were used in creating this project:
- python==2.7.18
- matplotlib==3.5.1
- numpy==1.22.0
- pandas==1.3.5
- seaborn==0.11.2

### 3. Project Motivation<a id="motivation"></a>

#### Scenario:
Working as a data analyst for an online food ordering and food delivery platform, I've been told by the Chief Marketing Officer that recent marketing campaigns have not been as effective as they were expected to be. I will analyze the data set to understand this problem and propose data-driven insights and recommendations.

As per Udacity, after completing this project, I was able to:
- Supplement statistics with visualizations to build an understanding of the data.
- Choose appropriate plots, limits, transformations, and aesthetics to explore a dataset, which allowed me to understand distributions of variables and relationships between features.
- Use design principles to create effective visualizations for communicating findings to an audience.

### 4. Key Files<a id="files"></a>
- `marketing_data.csv`\
Rather than use a tidy dataset provided by Udacity, I chose an external dataset because of its connection to sales and marketing--a topic I am interested in. This dataset was downloaded from a [kaggle dataset](https://www.kaggle.com/jackdaoud/marketing-data) and consists of 2,240 customers of an online food ordering and food delivery platform. The dataset contains data on:
    - Customer profiles
    - Product preferences
    - Campaign successes/failures
    - Channel performance
    
    The data was untidy and required thorough cleaning. The final, tidy dataset is saved as `marketing_cleaned.csv`.

- `Part_I_exploration.ipynb` and `Part_I_exploration.html`\
In part 1, exploratory data analysis, I conducted the bulk of my project in a Jupyter Notebook. Everything from assessing, wrangling, cleaning, and exploring the data was done here. As per the assignment, I structured my exploratory analysis sequentially from univariate analysis, bivariate analysis, then finally to multivariate analysis. I was searching for correlations relationships between many of the numerical and categorical variables which lead to the creation of over 30 visualizations. 

- `Part_II_slide_deck.ipynb` and `Part_II_slide_deck.slides.html`\
In part 2, explanatory data analysis, I selected the visualizations that could be grouped together to form clear insights. From the jupyter notebook, I created a slide deck to easily communicate my findings and recommendatsions to the Chief Marketing Officer. 

### 5. Summary of Findings<a id="summary"></a>

- There was a strong positive relationship between income and educational level.
- Wine was the most popular product, amounting to over 50% of sales. 
- Doctorates particularly enjoy wine. Doctorates from Germany especially. 
- Out of the 7 countries survey, a huge majority come from Spain, which perhaps accounts for the popularity of wine and meat.
- Surprisingly, those with 0 dependents had the highest income, and therefore spent the most and made the most purchases.
- Unsurprisingly, those with only high school education made fewer purchases and spent less in general.
- The most recent campaign was the most successful while #2 campaign was the least successful.
- Most customers still preferred shopping in-store rather than using catalogs.

### Key Insights for the Slide-Deck Presentation

There were many threads to explore but I settled on 4 specific metrics to analyze. The number on the bulleted lists correspond to the sequence and title of the visualizations as they appeared in `Part_I_exploration.ipynb`.

1. Campaign success
    - #14 Number of campaign success and success rate (horizontal bar plots)
    - #25 Relationship between campaign success rate and country (facetted horizontal bar plots)
2. Sales channel
    - #11 Number of purchases by sales channel (histograms)
    - #12 Share of purchases by sales channel (horizontal bar plot)
    - #13 Average number of purchases per channel per ID (horizontal bar plot)
3. Purchasing trends
    - #8 Average amount spent per product per customer (horizontal bar plot)
    - #9 Share of spending by product type (horizontal bar plot)
4.  Number of dependents
    - #10 Number of dependents per household (bar plots)
    - #21 Correlation between numerical variables (heat map)
    - #22 Income, total amount spent, and total purchases vs number of dependents (regression plots)
    - #32 Relationship between income, total amount spent, and the number of dependents (categorical scatter plot)

Please see my [slide deck](https://keenan-cooper.github.io/Marketing-Analytics-for-a-Food-Delivery-Platform/Part_II_slide_deck.html) for an executive summary with the above visualizations.

### 6. Acknowledgements<a id="acknowledgements"></a>
This project was completed as part of the Udacity's [Data Analyst Nanodegree](https://github.com/keenan-cooper/WeRateDogs-Twitter-Data-from-2015-to-2017/files/7847764/nd002-syllabus_2018-June_v9.pdf).\
Credit to Dr. Omar Romero-Hernandez for providing this [kaggle dataset](https://www.kaggle.com/jackdaoud/marketing-data) for his students. And credit to Jack Daoud for uploading and maintaining this data on Kaggle.

