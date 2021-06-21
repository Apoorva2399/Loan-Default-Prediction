# Loan-Default-Prediction

### **Problem Statement Analysis**
Loan default occurs when a borrower fails to pay back a debt according to the initial arrangement. In the case of most consumer loans, this means that successive payments have been missed over the course of weeks or months. Fortunately, lenders and loan servicers usually allow a grace period before penalizing the borrower after missing one payment. The period between missing a loan payment and having the loan default is known as delinquency. The delinquency period gives the debtor time to avoid default by contacting their loan servicer or making up missed payments.
Defaulting on a loan will cause a substantial and lasting drop in the debtor's credit score, as well as extremely high interest rates on any future loan. For loans secured with collateral, defaulting will likely result in the pledged asset being seized by the bank. The most popular types of consumer loans that are backed by collateral are mortgages, auto loans and secured personal loans. For unsecured debts like credit cards and student loans, the consequences of default vary in severity according to the type of loan. In the most extreme cases, debt collection agencies can garnish wages to pay back the outstanding debt.
 
 ![Default-on-Loans](https://user-images.githubusercontent.com/81186352/122775848-2e7a6f00-d2c8-11eb-80a8-ac295439e4ea.jpg)

### Data Pipeline :
* Data processing-1: In this first part we’ve removed unnecessary features. Since there were many columns with more than 70% of null values.
* Data processing-2: In this part, we manually go through each features selected from part 1, And encoded the categorical features ,changed the columns containing date time values.
* EDA: In in this part, we do some exploratory data analysis (EDA) on the features selected in part-1 and 2 to see the trend.
* Create a model: Finally, In this last but not the last part, we create models. Creating a model is also not an easy task. It’s also an iterative process. we show how to start with a with a simple model, then slowly add complexity for better performance.

### Model Summary :
* Developed an XGBoost binary classifier to predict whether a customer will default on a loan and achieved the AUPRC scores of 92% and 88% on test data respectively.
* Basic data inspection by Exploratory Data Analysis using Matplotlib and Seaborn giving an in-depth intuition to the important features of our dataset.
* Missing value imputation using KNN-Imputer, implemented SMOTE boosting, and carried out hyperparameter tuning using Bayesian optimization.
* Obtained Model Reason Codes (MRCs) by leveraging the concept of SHAP plots to cater to customer grievances and analyzed the Gains table to decide rejection cutoff.

### Conclusion :
* The last_fico_range, grade, inq_last_6month features were found to be the most relevant for predicting loan default in. The current model tries to predict default biased data from credit analysts grade and assigned interest rate. . The XGB and Rf models provide substantial improvements on traditional credit screening. A recall score significantly and robustly above 90%, with AUC-ROC scores ≃74%. The features provided to the model in our study generalize to any lending activity and institution, beyond P2P lending. The present work could, therefore, be augmented in order to predict loan default risk without the need for human credit screening.
* Only the Random Forest., XGBoost, model is used, but there are many good ones out there even neural networks. The models can also be improved further by finer tunings on hyperparameter.
* In the bank loan behaviour prediction, for example, banks want to control the loss to a acceptable level, so they may use a relatively low threshold. This means more customers will be grouped as “potential bad customers” and their profiles will be checked carefully later by the credit risk management team. In this way, banks can detect the default behaviours in the earlier stage and conduct the corresponding actions to reduce the possible loss.


