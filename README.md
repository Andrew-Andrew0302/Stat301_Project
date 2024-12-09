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

This project explored whether there are income differences between men and women and how factors like job type and hours worked per week contribute to these disparities. We used a logistic regression model to predict whether an individual's income exceeds $50K annually, leveraging backward selection to identify the most significant predictors. Our analysis revealed that factors such as education level, marital status, job type, relationship status, capital gains, and capital losses were the most influential in predicting income. Interestingly, gender itself was not a significant predictor in the final model once these other variables were accounted for.

**Why Logistic Regression?**
Logistic regression was chosen because it is a well-suited method for binary classification problems, like predicting whether income exceeds $50K. Its interpretability is a significant strength, as it allows us to assess the direct impact of predictors on the probability of earning above the threshold. For example, the model provides odds ratios, which can help us understand how a unit increase in variables like education level or hours worked influences the likelihood of earning more.

Another reason for using logistic regression is its ability to handle both categorical and numerical predictors effectively. The dataset contains a mix of variable types (e.g., categorical variables like gender and education, and numerical variables like age and hours worked), which logistic regression can incorporate seamlessly without requiring extensive preprocessing.

**Model Performance and Limitations**
While the model performed well, achieving an accuracy of 83.32%, there are some limitations that could affect the validity of our conclusions:

Imbalanced Data: The dataset contained more individuals earning less than $50K than those earning above it. This imbalance may have caused the model to favor the majority class, potentially skewing predictions. Techniques like oversampling the minority class or using a weighted loss function could help address this issue in future analyses.

Outliers in Capital Gains and Losses: Extreme values in capital gains and losses may have disproportionately influenced the model's predictions. These outliers were not removed or transformed in the analysis, which could distort the estimated relationships between predictors and the outcome. Future work should consider removing or handling outliers using robust techniques.

Variable Selection: Backward selection was used to refine the model, but it might not always lead to the most optimal set of predictors. Other selection methods, such as forward selection or stepwise regression, or even regularization techniques like Lasso regression, could be explored to ensure that the final model is both parsimonious and effective.

Interactions Between Variables: The logistic regression model did not account for possible interactions between variables, such as the combined effect of education level and job type on income. Including interaction terms could uncover more nuanced relationships and improve the model's explanatory power.

**Future Directions**
Future studies could address some of these limitations to build on our findings. For instance, testing more complex models like random forests or gradient boosting machines could capture non-linear relationships and interactions between variables, potentially improving predictive performance. Additionally, incorporating data on workplace policies, cultural norms, or access to childcare could provide a broader context for understanding income disparities.

**Conclusion**
Although gender was not a significant predictor in the final model, our findings highlight the structural factors, such as education level and job type, that contribute to income differences. These results suggest that addressing income inequality may require targeted interventions to reduce barriers to education and increase access to higher-paying job opportunities for underrepresented groups. By refining our analysis and incorporating additional data in future research, we can work toward a more comprehensive understanding of income disparities and how to mitigate them effectively.


**Reference**

Becker, B. & Kohavi, R. (1996). Adult [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5XW20.     

Graf, N. (2024, April 14). Gender pay gap in U.S. hasn’t changed much in two decades. Pew Research Center. https://www.pewresearch.org/short-reads/2023/03/01/gender-pay-gap-facts/ 

Schneider, S., Rentzsch, K., & Schütz, A. (2022). The gender pay gap is smaller in occupations with a higher ratio of men: Evidence from a national panel study. PLoS ONE, 17(7), e0270343. https://doi.org/10.1371/journal.pone.0270343 

