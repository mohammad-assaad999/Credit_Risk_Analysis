# Credit_Risk_Analysis
## Overview of the loan prediction risk analysis
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I've oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I've used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I've compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results
### Oversampling
 ![image](https://user-images.githubusercontent.com/80184581/129283877-82e0b6a0-c23b-4837-ab03-2cc67bcb2f60.png)
 - **Accuracy Score:** The classifier is 66.03% correct with the model which is considered a low accuracy.
 - **Precision:** Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk level is 1% and 100% for the low risk. The precision for the high risks is low which indicates that a large number of the high risks are false positives.
 - **Recall:** Recall is the ability of the classifier to find all the positive samples. It is 74% for the high risk and 58% for the low risk. A low recall is indicative of a large number of false negatives.

### SMOTE Oversampling
 ![image](https://user-images.githubusercontent.com/80184581/129284983-ed381e2c-74ae-4ec1-9390-dcc5e64716c7.png)
 - **Accuracy Score:** The classifier is 65.37% correct with the model which is considered a low accuracy.
 - **Precision:** Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk level is 1% and 100% for the low risk. The precision for the high risks is low which indicates that a large number of the high risks are false positives.
 - **Recall:** Recall is the ability of the classifier to find all the positive samples. It is 62% for the high risk and 68% for the low risk. A low recall is indicative of a large number of false negatives.

### Undersampling
 ![image](https://user-images.githubusercontent.com/80184581/129285092-a1ed2d9e-27e1-48fa-8df8-d56e8c769968.png)
 - **Accuracy Score:** The classifier is 58.52% correct with the model which is considered a low accuracy.
 - **Precision:** Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk level is 1% and 100% for the low risk. The precision for the high risks is low which indicates that a large number of the high risks are false positives.
 - **Recall:** Recall is the ability of the classifier to find all the positive samples. It is 64% for the high risk and 53% for the low risk. A low recall is indicative of a large number of false negatives.

### Combination (Oversampling & Undersampling)
 ![image](https://user-images.githubusercontent.com/80184581/129285198-263266e5-ab23-4fc2-bf37-878fd8d16797.png)
 - **Accuracy Score:** The classifier is 58.52% correct with the model which is considered a low accuracy.
 - **Precision:** Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk level is 1% and 100% for the low risk. The precision for the high risks is low which indicates that a large number of the high risks are false positives.
 - **Recall:** Recall is the ability of the classifier to find all the positive samples. It is 72% for the high risk and 57% for the low risk. A low recall is indicative of a large number of false negatives.

### Balanced Random Forest Classifier
 ![image](https://user-images.githubusercontent.com/80184581/129285446-0d7d0cc2-3e4f-43cf-9f37-52d8bee346b4.png)
 - **Accuracy Score:** The classifier is 95.54% correct with the model which is considered a high accuracy.
 - **Precision:** Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk level is 6% and 100% for the low risk. The precision for the high risks is low which indicates that a large number of the high risks are false positives.
 - **Recall:** Recall is the ability of the classifier to find all the positive samples. It is 100% for the high risk and 91% for the low risk. A high recall is indicative of a small number of false negatives.

### Easy Ensemble AdaBoost Classifier
 ![image](https://user-images.githubusercontent.com/80184581/129285636-468d97c1-a88f-44d5-9680-7009162398d1.png)
 - **Accuracy Score:** The classifier is 93.17% correct with the model which is considered a high accuracy.
 - **Precision:** Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk level is 9% and 100% for the low risk. The precision for the high risks is low which indicates that a large number of the high risks are false positives.
 - **Recall:** Recall is the ability of the classifier to find all the positive samples. It is 92% for the high risk and 94% for the low risk. A high recall is indicative of a small number of false negatives.

## Summary
To summarize, the first four models have very bad results where the accuracu scores, precision, and recalls are very low. However, the scores are very high in the last two models (Balanced Random Forest Classifier & Easy Ensemble AdaBoost Classifier) which makes it more reasonable for us to use them. 
