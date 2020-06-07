# COMPAS Recidivism Data Analysis

By: Ethan Wong, Kyle Mettler, Tyler Rosselli

Many judges, probation officers, and parole officers are beginning to use algorithms to try and see if criminals are likely to re-commit crimes, and one of the most popular algorithms for this is COMPAS (Correctional Offender Management Profiling for Alternative Sanctions).

Our Question: With algorithms such as these, bias is a common factor that may influence greatly the recidivism scores presented by the algorithm. This is extremely important as the COMPAS algorithm could potentially be affecting the livelihood of convicts that are trying to change for the better. Therefore, we want to ask, is the data produced by the COMPAS algorithm biased in terms of race?

Our Solution: 
- The data that we used for this project was in 2 parts: a raw data file, and a two-year data file that showed whether or not the convicts actually ended up recommitting crimes in the span of 2 years.
- Starting with the raw file, we cleaned the data and performed EDA and hypothesis tests to see how factors such as decile score (a score from 1-10 to show the likelihood of convicts recommitting crimes, 10 being the highest) and recommended supervision level were distributed amongst the races given in our data. We then repeated the process on the two-year data file.
- We then ran machine learning models on our existing clean data and used confusion matrices to look for false positives and false negatives that our models were predicting as concrete proof for the bias in our data.

Our Answer: We conclude, through our findings, that the data is indeed biased towards African Americans.
hi
