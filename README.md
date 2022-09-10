# Credit Risk Analysis

## Overview of the analysis
#### The purpose of this project is to solve a credit card risk challenge by applying machine learning. 
#### In this sense, ***imbalanced-learn*** and ***scikit-learn*** techniques are used to build and evaluate models using resampling. 
#### Besides,  ***RandomOverSampler*** and ***SMOTE*** algorithms are used to oversample the data, while ***ClusterCentroids*** algorithm is used to undersample the data. 
#### As requested, a combinatorial approach of over and undersampling is performed by usign ***SMOTEENN*** algorithm. 
#### To predict credit risk, the two new machine learning models that reduce bias (***BalanceRandomForestClassifier*** and ***EasyEmsembleClassifier***) are compared. 
#### Additionally, a recommendation on whether these models should be used to predict credit risk is requested. 

---
## Results

<table class="t1" 
<thead>
<tr><th> Models </th><th> Accuracy </th><th> Precision </th><th> Sensitivity (Recall) </th><th> F1 Score </th></tr>
</thead>
<tbody>
<tr><td>Random Oversampling</td><td>0.6366972052004142</td><td>0.99</td><td>0.65</td><td>0.79</td></tr>
<tr><td>SMOTE Oversampling</td><td>0.6302712208564487</td><td>0.99</td><td>0.64</td><td>0.78</td></tr>
<tr><td>Cluster Centroids Undersampling</td><td>0.6302712208564487</td><td>0.99</td><td>0.44</td><td>0.60</td></tr>
<tr><td>SMOTEENN Combination Sampling</td><td>0.6527933894952278</td><td>0.99</td><td>0.59</td><td>0.74</td></tr>
<tr><td>Balanced Random Forest Classifier</td><td>0.67209249388625</td><td>1.00</td><td>1.00</td><td>1.00</td></tr>
<tr><td>Easy Ensemble AdaBoost Classifier</td><td>0.925427358175101</td><td>0.99</td><td>0.94</td><td>0.97</td></tr>
</tbody>
</table>



+ ***RANDOM OVERSAMPLING Model***



+ ***SMOTE OVERSAMPLING Model***
+ ***CLUSTER CENTROIDS UNDERSAMPLING Model***
+ ***SMOTEENN COMBINATION SAMPLING***
+ ***BALANCED RANDOM FOREST CLASSIFIER Model***
+ ***EASY ENSEMBLE AdaBoost CLASSIFIER Model***


## Summary

The recommended model to use to predict the credict risk is Easy Ensemble AdaBoost Classifier. This model shows the highest accuracy rate with 0.925427358175101, as well as high rates of precision (0.99), sensitivity (0.94), and the F1 score at 0.97 is also high. 