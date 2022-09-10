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

![D](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D.png)


+ ***RANDOM OVERSAMPLING Model***
![D11](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D11.png)

+ ***SMOTE OVERSAMPLING Model***
![D12](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D12.png)

+ ***CLUSTER CENTROIDS UNDERSAMPLING Model***
![D13](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D13.png)

+ ***SMOTEENN COMBINATION SAMPLING***
![D14](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D14.png)

+ ***BALANCED RANDOM FOREST CLASSIFIER Model***
![D21](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D21.png)

![D22](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D22.png)

+ ***EASY ENSEMBLE AdaBoost CLASSIFIER Model***
![D23](https://github.com/Connectime4ever/Credit_Risk_Analysis/blob/main/D23.png)



## Summary

As the outputs of all the models run are non continue but discrete values, in this particular case the accuracy rate is not the best way to assess the model performance.  Therefore, the recommended model to use to predict the credit risk is the  Balanced Random Forest Classifier model. This model shows a precision rate and a sensitivity rate of 1.0, hence a perfect F1 score of 1.0.  

