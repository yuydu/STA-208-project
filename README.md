# STA 208 Project

## Application of Classification Methods in Analyzing and Predicting Loan Status

data source: https://www.lendingclub.com/info/download-data.action

Procedures:

## 1. Introduction

## 2. Variable Selection and Data Discription

### 2.1 Variable Selection Using Group Lasso

### 2.2 Numerical Variables Description
In this part we explore relationship among selected numerical predictor variables(computing correlation matrix and drawing heatmap). Relationship between loan status and some predictor variables we are interested in is also analyzed.(You are able to see the analysis procedure and results at [Numerical](https://github.com/yuydu/STA-208-project/blob/master/Variable%20Selection%20and%20Data%20description.ipynb),part 2.4.1)

### 2.3 Categorical Variables Description
For  selected  dummy  variables,  counter  barplot  for  pairs  of  each  categorical  variable  and  loan  status  weredraw sequentially. (You are able to see the analysis procedure and results at [Categorical](https://github.com/yuydu/STA-208-project/blob/master/Variable%20Selection%20and%20Data%20description.ipynb),part 2.4.2)

### 2.4 Principal Component Analysis
We use Principal Component Analysis(PCA) method to obtain a clearer interpretation of the differences between borrowers that lead to different loan status. The number of principal components is decided as 10, and a Varimax Rotation is implemented to recogonize the most powerful componetns.

Details in [PCA, KNN and Random Forest Clsifier.ipynb](https://github.com/yuydu/STA-208-project/blob/master/PCA%2C%20KNN%20and%20Random%20Forest%20Clsifier.ipynb)

## 3. Model Building and Selection

### 3.1 Support Vector Machines
In this part SVM is chosed to do calssification od loan status. Results show that test error is 0.0338 and accuracyscore is 0.9661 , which means our model fits the data well. Moreover, ROC area is 0.87, indicating high prediction accuracy and PR curve also shows high precision and high recall value.(You are able to see the analysis procedure and results at [SVM](https://github.com/yuydu/STA-208-project/blob/master/SVM.ipynb))


### 3.2 Logistic Regression

### 3.3 KNN Classification
K-nearest-neighbor Classifier is also applied to predict the loan status. The tuning parameter \textbf{k} (number of neighbors) is determined by computing the misclassification rate on the testing set by fitting the classifier on the training set. The test error picks k = 8. And the model predicts about 95% of the data right.

Details in [PCA, KNN and Random Forest Clsifier.ipynb](https://github.com/yuydu/STA-208-project/blob/master/PCA%2C%20KNN%20and%20Random%20Forest%20Clsifier.ipynb)

### 3.4 Random Forest Classification
We implement the random forest classifier with the number of trees prespecified as 1000, and compute the misclassification rate of prediction on the testing set. The accuracy rate is over 97%.

Details in [PCA, KNN and Random Forest Clsifier.ipynb](https://github.com/yuydu/STA-208-project/blob/master/PCA%2C%20KNN%20and%20Random%20Forest%20Clsifier.ipynb)

## 4. Conclusion
### 4.1 Model Decision
According to prediction accuracy on testing set of four fitted models, __Random Forest Classifier__ has highest accuracy, which predicts 97.1% of the data to be in loan status. Then we want to apply this model into future prediction in reality. 

### 4.2 Future Prediction
We use above models to do prediction in reality. However, results are not so good as expected. Random Forest Classifier only predicts about 30% as in good status abd SVM predict 67%. Here logistic preforms best as there are about 75% good-status loans. We also expkore why does it happen, whose result can be seen at  
[PredictionUsingRandomForest.ipynb;](https://github.com/yuydu/STA-208-project/blob/master/PredictionUsingRandomForest.ipynb)   [Prediction in Reality;](https://github.com/yuydu/STA-208-project/blob/master/SVM.ipynb)  
[Logistic](https://github.com/yuydu/STA-208-project/blob/master/Logistic%20Regression%20and%20Prediction%20in%20Reality.ipynb)

