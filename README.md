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

### Undersampling
<img width="511" alt="Undersampling Balanced Accuracy Score" src="https://user-images.githubusercontent.com/96451672/166149109-d00dec98-3c07-4b56-af73-ab69fac79530.png">
<img width="841" alt="Undersampling Imbalanced Classification Report" src="https://user-images.githubusercontent.com/96451672/166149111-bb747a7f-f34e-43fa-84eb-ae8025301d23.png">

* The balanced accuracy score is 52.9%.
* The precision scores were again the same as both of the oversampling models. High risk loans had a low precision score indicating a large number of false positives. Low risk loans had a very high precision score with all accurately predicted.
* While comparing to the oversampling models, the recall score for high risk loans remained higher at .61 and the recall score for low risk loans dropped quite a bit to .45 indicating lower accuracy in predicting positive low risk loans.

### Combination (Over and Under) Sampling
<img width="538" alt="Combination Sampling Balanced Accuracy Score" src="https://user-images.githubusercontent.com/96451672/166149717-bb63620d-8ded-4be8-8f5a-297b80e68dd5.png">
<img width="817" alt="Combination Sampling Imbalanced Classfication Report" src="https://user-images.githubusercontent.com/96451672/166149722-5d9ac97b-14e5-4b63-8d9f-ba082fb40837.png">

* The balanced accuracy score is 63.7%.
* The precision scores were once again the same as both of the oversampling models and the undersampling model. High risk loans had a low precision score indicating a large number of false positives. Low risk loans had a very high precision score with all accurately predicted.
* The recall score for high risk loans is again higher at .70 and the recall score for low risk loans is lower at .57 which continues to indicate lower accuracy in predicting positive low risk loans.

### Balanced Random Forest Classifier
<img width="499" alt="Balanced Random Forest Classifier Balanced Accuracy Score" src="https://user-images.githubusercontent.com/96451672/166150040-0befbbc5-c316-4e1d-b099-fbb868f76237.png">
<img width="818" alt="Balanced Random Forest Classifier Imbalanced Classification Report" src="https://user-images.githubusercontent.com/96451672/166150043-e61ddb15-9b0b-4676-9028-fc77335bcb42.png">

* The balanced accuracy score is 78.7%.
* The precision score adjusted slightly higher for high risk loans but still remained low at .04. The precision score for low risk loans remained the same with all accurately predicted.
* The recall score for low risk loans dramatically increased to .90 while the recall score for high risk loans remained relatively similar at .67.


### Easy Ensemble AdaBoost Classifier
<img width="482" alt="Easy Ensemble AdaBoost Classifier Balanced Accuracy Score" src="https://user-images.githubusercontent.com/96451672/166150616-048bc3b8-18ca-46cb-bdec-64e0bc7de22a.png">
<img width="807" alt="Easy Ensemble AdaBoost Classifier Imbalanced Classification Report" src="https://user-images.githubusercontent.com/96451672/166150622-4660ff26-fce0-482b-8aad-c5b4d69f33c0.png">

* The balanced accuracy score is 92.5%.
* The precision score adjusted slightly higher again for high risk loans at .07 and low risk loans all accurately predicted.
* The recall score for both low risk and high risk loans dramatically increased with low risk loans at .94 and high risk loans remaat .91.
