# Classification Report

Project Title : Credit Risk Prediction Using Machine Learning Models  
Objective: To predict the likelihood of a customer defaulting on a credit card.

# Evaluation Metrics Used

- Accuracy: Overall correctness of the model  
- Precision: How many predicted defaulters (1s) were actually defaulters.
- Recall: How many actual defaulters were identified correctly.
- F1 Score: Harmonic mean of precision and recall  
- Confusion Matrix: Matrix to visualize true vs predicted classifications

# Model 1: Logistic Regression

-Accuracy: 0.6678333333333333
-Precision: 0.35817717206132876
-Recall: 0.6337603617181613
-F1 Score: 0.457687074829932

-Confusion Matrix:
 [[3166 1507]
 [ 486  841]]

-Classification Report:
               precision    recall  f1-score   support

         0.0       0.87      0.68      0.76      4673
         1.0       0.36      0.63      0.46      1327

    accuracy                           0.67      6000
   macro avg       0.61      0.66      0.61      6000
weighted avg       0.75      0.67      0.69      6000

-AUC-ROC Score: 0.7098910817179807

# Model 2: Random Forest Classifier

-Accuracy: 0.814
-Precision: 0.6393659180977543
-Recall: 0.36473247927656366
-F1 Score: 0.46449136276391556

-Confusion Matrix:
 [[4400  273]
 [ 843  484]]
 
-Classification Report:
               precision    recall  f1-score   support

         0.0       0.84      0.94      0.89      4673
         1.0       0.64      0.36      0.46      1327

    accuracy                           0.81      6000
   macro avg       0.74      0.65      0.68      6000
weighted avg       0.80      0.81      0.79      6000

-AUC-ROC Score: 0.7465857913899066

# Model 3: Support Vector Machine (SVM)

-Accuracy Score: 0.8141666666666667
-Precision: 0.6424731182795699
-Recall: 0.3602110022607385
-F1 Score: 0.46161274746499276

-Classification Report:
              precision    recall  f1-score   support

         0.0       0.84      0.94      0.89      4673
         1.0       0.64      0.36      0.46      1327

    accuracy                           0.81      6000
   macro avg       0.74      0.65      0.67      6000
weighted avg       0.80      0.81      0.79      6000

-Confusion Matrix:
[[4407  266]
 [ 849  478]]


# Model 4: Decision Tree Classifier

-Accuracy: 0.7321666666666666
-Precision: 0.42473118279569894
-Recall: 0.5953278070836473
-F1 Score: 0.4957640414182617

-Classification Report:
               precision    recall  f1-score   support

         0.0       0.87      0.77      0.82      4673
         1.0       0.42      0.60      0.50      1327

    accuracy                           0.73      6000
   macro avg       0.65      0.68      0.66      6000
weighted avg       0.77      0.73      0.75      6000

-Confusion Matrix:
[[3603 1070]
 [ 537  790]]


# Model 5: XGBClassifier

-Accuracy: 0.7998333333333333
-Precision: 0.565625
-Recall: 0.4091936699321778
-F1 Score: 0.474857892435505

-Classification Report:
               precision    recall  f1-score   support

         0.0       0.84      0.91      0.88      4673
         1.0       0.57      0.41      0.47      1327

    accuracy                           0.80      6000
   macro avg       0.71      0.66      0.68      6000
weighted avg       0.78      0.80      0.79      6000

-Confusion Matrix:
[[4256  417]
 [ 784  543]]

# Conclusion

Among the models tested:
- "Random Forest" performed best with high accuracy and precision.
- SVM and Random Forest performed comparably.
- Model selection may vary based on the test data size, class distribution, and overfitting risks.
- If to avoid wrong classification(non-defaulters as defaulters) we can choose Random Forest.
