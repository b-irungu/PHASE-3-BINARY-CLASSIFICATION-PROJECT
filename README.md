# SYRIATEL COMPANY CUSTOMER CHURN ANALYSIS PROJECT

USING BINARY CLASSIFICATION TO BUILD A MODEL THAT ACCURATELY PREDICTS CUSTOMER CHURN TO HELP SYRIATEL COMPANY IDENTIFY THE FACTORS CONTRIBUTING TO THE CHURN AND TAKE PROACTIVE ACTIONS TOWARDS RETAINING THEIR CUSTOMERS

**OVERVIEW**

This is a binary classification project that conducts a chrn analysis for SyriaTel which is a telecommunication company in Syria. The project aims at identifying the factors that contribute to curstomer churn and Develop a classifier that predicts which customers are likely to churn to enable SyriaTel take appropriate actions and reduce customer attrition.

**DATA**

This project uses the SyriaTel Customer churn data set which is retrieved from Kaggle: https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset. The dataset is suitable for this project based on the following aspects;

* It contains comprehensive information on various features of the telecommunication services provided by the company including account length, area code, phone number, international plan, voice mail plan, and various other features related to customer usage patterns.
* The data set also contains the feature 'churn,' which indicates whether a customer has churned or not which will be used as the target variable making the dataset suitable for analyzing customer churn as it contains all the necessary information to develop a predictive model.
* The data he dataset is large enough, with over 3,000 records, to support the development of a reliable and accurate predictive model. 

**METHOD**

The project used the CRIPSM-DM data science process to analyse and create a model best for the churn analysis. the projects used the following Binary classifiers
* KNN(K-Nearest Neighbours)
* Logistic Regression
* Decision Trees
* Random Forest

**FINDINGS**

The findings of the various classifiers used in this project are as follows:

**KNN findings**

This classifiers had the lowest perfomance(based on the recall evaluation), as the recall score ws 13.91%. with this score the model had a high rate of producing false negative churns which would result to mislead decision making if the same was adopted. 

**Logistic Regression findings**

The recall score for the clssifier was 28% which also indicated that the clasifier erfomed poorly on correctly predicting customer churn, thus the classifier could not be adopted

**Decision Trees findings**

With an accuracy of 0.826, precision of 0.826, recall of 0.826, and F1-score of 0.826, the decision tree classifier trained using highly correlated variables with the target variable performed quite well.

**Random Forest Findings**

**CONCLUSION**

**BUSINESS RECOMMENDATION**
