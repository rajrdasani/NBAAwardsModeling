# NBA Awards Modeling
# Making Subjective NBA Awards Objective: Predicting NBA End-of-Season Awards with Statistics


This project implements machine learning and data analytics methodologies to predict winners of six individual, end-of-season NBA Awards. 


## Project Objective


The primary objective of this project is to create an objective prediction model for each of the 5 main NBA Awards: Most Valuable Player (MVP), 6MOY (6th Man of the Year), DPOY (Defensive Player of the Year), ROY (Rookie of the Year), and MIP (Most Improved Player).


## Model Algorithms and Methods Used
* Linear Regression
* Ridge Regression
* Lasso Regression
* Random Forest


## Technologies and Packages Used
* R, Python, Jupyter Notebook
* Python: NumPy, Pandas, Sklearn, Matplotlib, StatsModels API
* R: dplyr, glmnet, stringi


## Pre-Filtered Datasets 
* nbaStats[Year].csv
   * Unfiltered NBA player statistics from basketball-reference for the years 2010-2020


## Cleaned and Filtered Datasets 
* update142.csv
   * 2010-2020 stats for each eligible NBA player including their voting percentages for each award
* roydata142.csv
   * 2010-2020 stats for each eligible Rookie of the Year player
* smoydata142.csv
   * 2010-2020 stats for each eligible Sixth Man of the Year player
* mip_stats.csv
   * 2011 -2020 difference in stats from the previous season for each eligible Most Improved Player player
* nba2021.csv
   * 2021 stats for each player (used for MVP and DPOY) 
* roy2021.csv
   * 2021 stats for each eligible Rookie of the Year Player
* smoy2021.csv
   * 2021 Stats for each eligible 6th Man of the Year Player
* mip2021.csv
   * Difference between 2021 and 2020 stats for each player up until 5/12/2021 (used for MIP) 


## Usage
The following steps should be taken to run the four regression models:
1. Start with The NBA Awards Data Cleaning file 
   1. Contains a step-by-step guide on the process and tools used to clean the data, including string manipulation, filtering, and handling missing variables. It can be run by downloading the nbaStats[Year].csvs. 
2. Create MIP data 
   1. MIP Creation file provides the code for this 
3. Choose your fighter (model), and load the data in (all the files includes commented code explaining each part): 
   1. Linear Regression: Linear Regression.ipynb
   2. Random Forest: RandomForests.ipynb
   3. Lasso + Ridge Regression: Lasso + Ridge Models.Rmd


## Contributors
Nilay Agarwalla, Raj Dasani, Bikram Khaira, Kenny Tran, Sarah Truong


## Acknowledgements
Thank you to Basketball Reference and the official NBA website for providing the datasets used in this analysis. Thank you to the IEOR 142, Introduction to Machine Learning and Data Analytics, course staff for their guidance throughout this project. 


## Resources
All data for 2020 (For all datasets, change the year in the URL to get different years): 
1. Player Data:https://www.basketball-reference.com/leagues/NBA_2020_per_game.html 
2. Voting Shares: https://www.basketball-reference.com/awards/awards_2020.html


Article Inspiration: 
1. https://towardsdatascience.com/predicting-2020-21-nbas-most-valuable-player-using-machine-learning-24aaa869a740 
2. https://towardsdatascience.com/using-data-science-to-predict-the-next-nba-mvp-30526e0443da 
3. https://dribbleanalytics.blog/2019/04/ml-mvp-all-nba-predict-2019/
