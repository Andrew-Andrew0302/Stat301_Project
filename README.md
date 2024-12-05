# Stat301_Project

**Introduction**
Income disparity between genders has long been a subject of social and economic research, with debates centered on the persistence of these differences and the factors that influence them.  Research by Schneider highlights that women earn less on average than men, even when controlling for working hours, leadership roles, and education, but adjusting for variables like working hours reduces the income gap, emphasizing the significant role of working patterns in shaping earnings(Schneider, 2022).  Graf complements this by noting that men are more likely to work full-time and hold leadership positions, both associated with higher pay(Graf , 2024).  Additionally, parenthood plays a critical role, with mothers often working fewer hours than fathers, further influencing earnings disparities.

For our group project, we utilized a dataset named "Adult " available at (https://archive.ics.uci.edu/dataset/2/adult).This dataset includes multiple variables that could potentially influence income, which is the target variable.         Here’s a summary of the variables:

Age: The age of the individual

Workclass: Type of WorkSector

fnlwgt: weighted tallies of any specified socio-economic characteristics of the population.

education: Education Level (Categorical)

Education.        num: Education-level (numeric)

Martial.        status: Martial Status of that individual

Occupation: Current job of that individual

Relationship: Relationship Status of that individual

Race: Race of that individual

Sex: Gender of that individual

Capital.        gain: Capital gains (Additional income from income)

Capital.        loss: Capital losses

Hours.per.week: Hours per week an individual works for

Native.        country: Country of origin for that individual

Income: Income category indicating if the individual earns more or less than $50K

The central question we aim to investigate Is there a significant income disparity between male and female individuals, and how do other factors like occupation and hours worked per week influence this disparity.        We plan to arrive at our final conclusion by using a Logistic Regression model to predict whether an individual's income exceeds $50K annually to create inference study.   we will use backwards selection way and confusion matrix to show the model to help draw conclusions regarding the impact of gender disparities on income and the role of factors such as occupation and hours worked per week.

**Discussion**

This project looked at whether there are income differences between men and women and how factors like job type and hours worked per week play a role. Using a logistic regression model, we found that factors such as education level, marital status, job type, relationship status, capital gains, and capital losses were the most important predictors of income (>50K). Surprisingly, gender itself wasn’t one of the key factors in the final model.

Our initial analysis showed that men are more likely to earn over $50K than women. However, when other factors like education and job type were considered, gender’s influence on income became less important. This suggests that income differences might be more about structural issues, like the kinds of jobs or education levels people have, rather than gender alone.

The model had an accuracy of 83.32%, meaning it performed well in predicting income. However, some issues, like imbalanced data (more people earning less than $50K) and extreme values in capital gains and losses, might have affected the results. Improving the model by adding interactions between variables or trying other methods like random forests could make it better.

Future studies could explore why certain jobs or education levels have such a big impact on income. Adding more data about workplace policies or cultural factors could also help us understand income differences better. These findings are a step toward identifying ways to reduce income inequalities.

**Reference**

Becker, B. & Kohavi, R. (1996). Adult [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5XW20.     

Graf, N. (2024, April 14). Gender pay gap in U.S. hasn’t changed much in two decades. Pew Research Center. https://www.pewresearch.org/short-reads/2023/03/01/gender-pay-gap-facts/ 

Schneider, S., Rentzsch, K., & Schütz, A. (2022). The gender pay gap is smaller in occupations with a higher ratio of men: Evidence from a national panel study. PLoS ONE, 17(7), e0270343. https://doi.org/10.1371/journal.pone.0270343 

