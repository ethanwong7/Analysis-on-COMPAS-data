# COMPAS Recidivism Data Analysis

By: Ethan Wong, Kyle Mettler, Tyler Rosselli

Many judges, probation officers, and parole officers are beginning to use algorithms to try and see if criminals are likely to re-commit crimes, and one of the most popular algorithms for this is COMPAS (Correctional Offender Management Profiling for Alternative Sanctions).

Our Question: With algorithms such as these, bias is a common factor that may influence greatly the recidivism scores presented by the algorithm. This is extremely important as the COMPAS algorithm could potentially be affecting the livelihood of convicts that are trying to change for the better. Therefore, we want to ask, is the data produced by the COMPAS algorithm biased in terms of race, and is COMPAS itself accurate?

Our Solution: 
- The data that we used for this project was in 2 parts: a raw data file, and a two-year data file that showed whether or not the convicts actually ended up recommitting crimes in the span of 2 years.
- Starting with the raw file, we cleaned the data and performed EDA and hypothesis tests to see how factors such as decile score (a score from 1-10 to show the likelihood of convicts recommitting crimes, 10 being the highest) and recommended supervision level were distributed amongst the races given in our data. We then repeated the process on the two-year data file.
- We then ran various machine learning models on our existing clean data and used confusion matrices to look for false positives and false negatives that our models were predicting as concrete proof for the bias in our data.

Our Answer: We conclude, through our findings, that the data is indeed biased towards African Americans, and that COMPAS itself is a considerably inaccurate algorithm.

Notebooks:
- Raw_Data_Analysis : We cleaned and performed EDA on the raw dataset and drew insights
- Two_Year_Data_Analysis : We cleaned and performed EDA on the two year dataset and drew insights
- Logistic_Regression_Model : We modelled our data using a logistic regression and looked at false positive and false negative counts and rates
- Decision_Tree_Model : We modelled our data using a decision tree and looked at false positive and false negative counts and rates
- COMPAS_Ensemble_Methods : We used ensemble methods to select the most accurate model for our data, ran that model, and looked at FP and FN counts and rates
- Clustering_K-means_two_year : We divided our data into clusters as a model but found there were no natural groupings or clusters in our data
- Correlation_Analyses : This notebook contains hypothesis tests and EDA on the data and used the Steiger and Fisher methods to compare correlations
- Column_Manipulation_Notebooks : This folder contains two variations of our logistic regression. We ran logistic regressions and changed up the columns we used to see if it would affect our results (it did not), and also showed that the risk scores themselves are inherently biased
