![SYRIATEL LOGO](https://user-images.githubusercontent.com/122228492/236913666-80474769-3d8e-458d-a7ff-f8cd96f51962.PNG)

# SYRIATEL COMPANY CUSTOMER CHURN ANALYSIS PROJECT

**USING BINARY CLASSIFICATION TO BUILD A MODEL THAT ACCURATELY PREDICTS CUSTOMER CHURN TO HELP SYRIATEL COMPANY IDENTIFY THE FACTORS CONTRIBUTING TO THE CHURN AND TAKE PROACTIVE ACTIONS TOWARDS RETAINING THEIR CUSTOMERS**

**REPOSITORY OUTLINE**

This repository contains the follwing
* A jupyter notebook 
* A non technical presentation.
* A CRISP-DM report
* A README file
* SyriaTel Customer churn data
* SyriaTel company logo
* churn distribution visual

**OVERVIEW**

This is a binary classification project that conducts a chrn analysis for SyriaTel which is a telecommunication company in Syria. The project aims at identifying the factors that contribute to curstomer churn and Develop a classifier that predicts which customers are likely to churn to enable SyriaTel take appropriate actions and reduce customer attrition.

**DATA**

This project uses the SyriaTel Customer churn data set which is retrieved from Kaggle: https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset. The dataset is suitable for this project based on the following aspects;

* It contains comprehensive information on various features of the telecommunication services provided by the company including account length, area code, phone number, international plan, voice mail plan, and various other features related to customer usage patterns.
* The data set also contains the feature 'churn,' which indicates whether a customer has churned or not which will be used as the target variable making the dataset suitable for analyzing customer churn as it contains all the necessary information to develop a predictive model.
* The data he dataset is large enough, with over 3,000 records, to support the development of a reliable and accurate predictive model. 

**Target and predictor variables**

The data has various feaatures where `churn` was the target variable feature while the rest were the predictor variable features. the predictor variable features include the `state`, `account length`, `area code`, `phone number`, `international plan`, `voice mail plan`,`number vmail messages`,`total day minutes`, `total day calls`, `total day charge`, `total eve minutes`, `total eve calls`, `total eve charge`,`total night minutes`,`total night calls`,`total night charge`,`total intl minutes`,`total intl calls`,`total intl charge`and `customer service calls`


**Customer churn distribution**

![churn distribution](https://github.com/b-irungu/PHASE-3-BINARY-CLASSIFICATION-PROJECT/assets/122228492/00deabcf-7814-4b1a-944d-b1404ecd51f4)


**METHOD**

The project used the CRISP-DM data science process to analyse and create a model best for the churn analysis. All the data science steps are described in the CRISP-DM Report:(**insert link**). The projects used the following Binary classifiers
* KNN(K-Nearest Neighbours)
* Logistic Regression
* Decision Trees
* Random Forest

**FINDINGS**

The findings of the various classifiers used in this project are as follows:

**KNN findings**

This classifiers had the lowest perfomance(based on the recall evaluation), as the recall score ws 19.31%. with this score the model had a high rate of producing false negative churns which would result to mislead decision making if the same was adopted. 

![knn confusion matrix](https://github.com/b-irungu/PHASE-3-BINARY-CLASSIFICATION-PROJECT/assets/122228492/e93e7800-3e82-4e0b-b926-ab35c586795b)


**Logistic Regression findings**

The recall score for the clssifier was 28% which also indicated that the clasifier perfomed poorly on correctly predicting customer churn, thus the classifier could not be adopted

![logistic regresion confusion matrix](https://github.com/b-irungu/PHASE-3-BINARY-CLASSIFICATION-PROJECT/assets/122228492/145cad4d-956a-4075-871b-aaa331c6d87a)


**Decision Trees findings**

The model reported a high accuracy of 0.929 and a decent mix of precision and recall(83.54% and 65.34% respectively. 

![decision tree confusion matrix](https://github.com/b-irungu/PHASE-3-BINARY-CLASSIFICATION-PROJECT/assets/122228492/04187f37-007c-4e93-b2c6-8ae053b72534)

**Random Forest Findings**

Random Forest was the best Model based on Recall Metric which was 75%. 7.4% of the predictions are False Negatives which means that the model will 7.4% of the time 
predict that a customer will not churn yet the customer churns.

![random forest confusion matrix](https://github.com/b-irungu/PHASE-3-BINARY-CLASSIFICATION-PROJECT/assets/122228492/78f5a5f7-48e7-406f-8aad-f89cfdb95663)


**CONCLUSION**

Based on the findings, the business conclusion can be drawn as follows:

* Importance of Recall: In the context of predicting customer churn, the focus was placed on optimizing for Recall. By prioritizing Recall, the goal was to minimize the number of customers who are incorrectly classified as non-churners.
* Best Model: Among the models explored, the Random Forest Classifier performed the best since was able to correctly identify 75% of the customers who were likely to churn.
* Despite the success of the Random Forest Classifier, it still had a False Negatives rate of 7.4%. This means that approximately 7.4% of the time, the model predicted that a customer would not churn when they actually did churn. This level of False Negatives could have a significant impact on the business.
* Predicting customer churn is an ongoing process, and it is important to continuously refine and improve the model. Regularly monitoring the model's performance, collecting new data, and incorporating feedback from business stakeholders can lead to better predictions and more accurate identification of customers who are at risk of churning.

**BUSINESS RECOMMENDATION**

Determine the unique needs of the following customers and meet them; 
* Heavy daytime callers. Come up with tariff incentives for them 
* Customers with international plans. Come up with unique retention plans 
* Customers who frequently call customer service. Assist customers proactively to reduce the need to call.

