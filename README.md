# LogisticRegression

The project was to evaluate whether credit models in fintech companies can be transferable by testing on LendingClub’s and Prosper’s customer datasets using Logistic Regression. Also, to investigate the differences behind two companies’ decision making criteria with Logistic Regression model coefficients.

Two datasets were from LendingClub and Prosper from 2012 Q1 to 2014 Q1. Some of the variables are fico score, employement length, purpose of debt, etc. 

The size of LendingClub dataset is (193,686, 11)  and The size of Prosper dataset is (49,648, 11).

Procedures for model:
1. train on LC and test on LC
2. train on LC and test on Prosper
3. train on Prosper and test on Prosper
4. train on Prosper and test on LC

Some of the conclusions:
- Highest accuracy: 86% (train on LC and test on Prosper)
- Lowest accuracy: 50% (train on Prosper and test on LC)
- All models produced ROC AUC metrics only slightly higher than 0.5
- From the coefficient analysis, Prosper takes a more comprehensive approach (stricter) because unlike LendingClub, the coeffients on Propser's dataset is more even.
- FICO score matters more to LendingClub (higher coefficients for FICO) even though their FICO requirement is lower (based on research on website for credit score requirements)
- Prosper pays more attention to DTI ratio, purpose of the loan, and employment length since the coefficients of these variables are high
