# Credit_Risk_Analysis
## Overview of Project
### Purpose
The purpose of this project is to analyze lending data using different models to determine the best model to predict credit risk. The models used are oversampling, undersampling, combined over and under sampling, BalancedRandomForestClassifier, and EasyEnsembleClassifier.

## Results
The following is the results for the different models providing these scores:
* **Balanced accuracy score:** How often the classifier is correct.
* **Precision score:** The measure of how reliable a positive classification is.
* **Recall score:** The ability of the classifier to find all the positive samples.

### Naive Random Oversampling
<img width="619" alt="Naive Random Oversampling Balanced Accuracy Score" src="https://user-images.githubusercontent.com/96451672/166148101-799152b2-d014-4033-be19-c8b3c81b226c.png">
<img width="846" alt="Naive Random Oversampling Imbalanced Classification Report" src="https://user-images.githubusercontent.com/96451672/166148108-1fa9073c-fdf1-4c9a-a7bf-3f0a5f83149b.png">

* The balanced accuracy score is 64.9%.
* High risk loans had a low precision score indicating a large number of false positives. Low risk loans had a very high precision score with all accurately predicted.
* The model was better at predicting positive low risk loans at .68 than high risk loans at .62.

### SMOTE Oversampling
<img width="566" alt="SMOTE Oversampling Balanced Accuracy Score" src="https://user-images.githubusercontent.com/96451672/166148586-6c17b74f-f4da-4eba-87be-db6dfc9fc65a.png">
<img width="870" alt="SMOTE Oversampling Imbalanced Classification Report" src="https://user-images.githubusercontent.com/96451672/166148594-eb7ebc3c-ad5d-45e9-a3a2-4c7ea3c7bddd.png">

* The balanced accuracy score is 64.4%.
* The precision scores were the same as the naive random oversampling model. High risk loans had a low precision score indicating a large number of false positives. Low risk loans had a very high precision score with all accurately predicted.
* Like naive random oversampling, the model was better at predicting positive low risk loans at .66 than high risk loans at .63.

