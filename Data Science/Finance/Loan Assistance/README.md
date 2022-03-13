
To predict loan defaults for banks or money lending businesses machine learning can be of great
significance. This work aims to demonstrate possible application of machine learning in this
business. For the money lending company ZFS, according to statistics there is an increment of
200% in loan applications. As all the applications are handled manually it increases the workload
on employees as well as it might result in reduction in customer satisfaction and increased risk of
investing in Non-Performing Assets.
For the given problems possible solutions are as following:
1. Use multiple prediction algorithms to forecast loan default.
2. Perform feature selection and then pack the best appropriate predictive model for
loan default prediction.

Data Explanation
The dataset has 13 features with 398 observations for train data and 247 observations for the test
data related to clients who took out a loan for the company. Following are the features of the
dataset:
Loan_ID
Gender
Married
Dependents
Education
Self_Employed
ApplicantIncome
CoapplicantIncome
LoanAmount
Loan_Amount_Term
Credit_History
Property_Area
Loan_Status
Here Loan_Status is a dependent variable which identifies N when a borrower defaults on the
loan and Y otherwise.
In the Data Explanation process the most important stage is Data Preparation. This task is to turn
qualitative characteristics into quantitative characteristics. Here, at the end of this process it will
turn Loan_Status “Y” to “1” and “N” to “0”. As there are no other qualitative features, we will
move to basic descriptive analysis.
Feature Selection
According to basic descriptive analysis and using Correlation matrix to get basic idea of
important features in evaluating loan application.

From the correlation matrix we can suggest following:
1. Loan_Status highly depends on Credit_Hisotry as it reflects the history of the applicant..
2. LoanAmount and ApplicantIncome is tightly correlated as if applicant’s income is not
high enough the risk of loan not getting repaid is high.
3. The Educational status of the applicant also matters as it shows if the applicant has
graduated and has a reliable source of money to pay up the loan.
4. Marital status and number of dependents the applicant is also correlated to loan approval.
5. Gender of the applicant is really not important so we can always deduct it from the
consideration.
Most important features suggested:
● Credit History
● Education Status
● Marital Status
● Number of Dependants
● Employment Status
Here are the cross graphs of each feature with Loan_Status.

This graph shows that if the applicant has good credit history, the risk of loan not repaying is
extremely low, at the same time it is high risk if applicant’s credit history is not good.
This graph shows that if the applicant has graduated, in other words, has a good education, the
risk of losing money is really low, and if the educational status is not good enough, the risk of
losing money is high.

This graph is more on the neutral side as it has almost the same ratio in both marital status and
loan status. Still it might make a difference if there is a co applicant with good income.

This graph shows that if an applicant has too many dependents on it, it might increase the risk of
losing money.
Data Modeling
The modeling procedure includes selecting the models from the various predicted models.
RandomForest, GradientBoosting, ADABoost, and SVC. The quantity of data provided during
training increases the prediction model’s accuracy.
Following graphs show feature importance obtained using RandomForest, GradientBoosting, and
ADABoost classifiers.

Steps:
● Cleaning the training data
● Passing clean data for model training
● Applying it to Predictive models
● Giving test data to trained model
● Evaluating model
● Selecting model
● Predicting Loan default
Conclusion
To conclude, we discovered that the AdaBoost predictive model produces the best results. As for
the question regarding importance of feature selection, we obtained that ApplicantIncome is the
most important variable that predicts the loan default with highest accuracy. The further work for
this study is to develop models by deepening analysis used in the models.
