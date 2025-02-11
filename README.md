# Comparing Classifiers

## Overview

In this application, our goal is to compare the performance of different classifiers, namely K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. 

## Dataset

We will utilize a dataset related to marketing bank products over the telephone. 
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls for a term deposit product.
The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y)

Path: https://github.com/CoderNBR/Practical-Application-3/tree/main/data
	
The dataset with 41188 campaingns and 20 inputs

Features:
* age (numeric)
* job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
* marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
* education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
* default: has credit in default? (categorical: 'no','yes','unknown')
* housing: has housing loan? (categorical: 'no','yes','unknown')
* loan: has personal loan? (categorical: 'no','yes','unknown')
* contact: contact communication type (categorical: 'cellular','telephone')
* month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
* day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
* duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
* campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
* pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
* previous: number of contacts performed before this campaign and for this client (numeric)
* poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')
* emp.var.rate: employment variation rate - quarterly indicator (numeric)
* cons.price.idx: consumer price index - monthly indicator (numeric)
* cons.conf.idx: consumer confidence index - monthly indicator (numeric)
* euribor3m: euribor 3 month rate - daily indicator (numeric)
* nr.employed: number of employees - quarterly indicator (numeric)

Output variable (desired target):
* y - has the client subscribed a term deposit? (binary: 'yes','no')

## Approach

1. Importing Data
2. Data cleaning
    - Clean the column names if required
    - Duplicate Check
    - Missing Value Check
 
3. Do EDA
4. Outlier Treatment
5. Data Pre-processing
6. Modelling
	- K Nearest Neighbour (KNN)
    - Logistic regression (LR)  
    - Decision Tree (DT)
    - Support Vector Machines (SVM)
7. Evaluation
8. Comparision
9. Conclusion

## Visualizations

1. [Histograms](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/Histograms.png)
2. [Boxplot Age By Marital](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/BoxplotAgeByMarital.png)
3. [Boxplot Age By Marital and Housing](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/BoxplotAgeByMaritalHousing.png)
4. [CorrelationHeatmap](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/CorrelationHeatmap.png)
5. [KNN Precision Recall Curve](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/KNNPrecisionRecallCurve.png)
6. [KNN ROC Curve](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/KNNROCCurve.png)
7. [KNN Confusion Matrix without Param](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/KNNConfMatwithoutParam.png)
8. [KNN Confusion Matrix with Param](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/KNNConfMatwithParam.png)
9. [Logistic Regression Precision Recall Curve](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/LRPrecisionRecallCurve.png)
10. [Logistic Regression ROC Curve](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/LRROCCurve.png)
11. [Decison Tree](https://github.com/CoderNBR/Practical-Application-3/blob/main/images/DecisionTree.png)

  
## Evaluation

Comparision of simple Models without any params or tuning 

<img width="300" alt="" src="https://github.com/CoderNBR/Practical-Application-3/blob/main/images/ModelswithoutParams.png">

Improved Models with Params

<img width="900" alt="" src="https://github.com/CoderNBR/Practical-Application-3/blob/main/images/ImprovedModelwithParamSetting.png">


## Conclusion & Recommendation

Based on the analysis and results, the best model in this case is Logistic

## Repository Link (GitHub)

1. [GitHub Link for Project "Comparing Classifiers"](https://github.com/CoderNBR/Practical-Application-3)
2. [Jupyter Notebook](https://github.com/CoderNBR/Practical-Application-3/blob/main/PracticalApplication3.ipynb)








   
