In this project, we will primarily be using these datasets:

    Relevant Twitter dataset from Kaggle (2020)
    Government census data (2016-2020)
        Poverty
        Education
        Employment
        Demographics {population, race and ethnicity, sex and gender, age groups}
        Religion


The Goal: To determine voter breakdown of each county by percentage, thereby determining the popular vote and electoral college outcomes of the 2020 presidential election. 
Reach Goal: Using data from (2020-2024) to predict the popular vote and electoral college outcomes of the 2024 presidential election.

Stakeholders: 
Political Campaign Teams: Interested in understanding potential voting outcomes to strategize campaign efforts
Government Officials: Could be interested in insights for policymaking or understanding public sentiment.

KPIs: 
Accuracy of Predictions: Measure of how accurately our model predicts voting outcomes compared to actual results.
Model Performance Metrics: Evaluation metrics to assess model performance.
Feature Importance: Understanding the impact of different features (e.g., poverty rates, education levels) on the predictions.

The Plan:
We plan to use county level data to determine voting outcomes of 2020, by considering Twitter posts of 2020, and relevant factors such as poverty rate, education level, employment rate, etc, ideally from 2016 to 2020. 

We will attempt to determine the voting breakdown of each county, thereby determining the popular vote and electoral college outcome of 2020.

Time permitting, we will try and predict 2024 outcomes using our model with 2020-2024 data.


Explanation of Features in aggregate.csv:
    GEO_ID: Unique identifier attached to each county
    NAME: Name of the county
    total_pop: Total population of the county
    pop_18_30_pc: Percentage of people in the age range 18 to 30
    pop_60_up_pc: Percentage of people in the age range 60 and up
    pop_male_pc: Percentage of male population
    afr_amer_pc: Percentage of african american population
    amer_ind_pc: Percentage of american indian population
    asian_pc: Percentage of asian population
    latino_pc: Percentage of latino population
    white_pc: Percentage of white population
    *_delta: Change in percentage of * population from 2016 to 2019
    unemp_rate: Unemployment rate as a percentage of population
    unemp_delta: Change in unemployment rate from 2016 to 2019
    mean_hhi: Mean household income
    med_hhi: Median household income
    hs_deg: Percentage of the adult population with a high school or equivalent degree
    bac_deg: Percentage of the adult population with a bachelors degree
    democrat: Percentage of votes going to the democratic candidate
    republican: Percentage of votes going to the republican candidate

Other possible features:
    Population in ages grouped in periods of 5 year (e.g. 10-15 years, 15-20 years etc)
    Poverty rate in age groups
    Population under 1.5 times the poverty limit
    Employment status for various age groups
    Employment status with respect to military jobs
    Male population in different age groups
    Number of people with mixed ethnicities
