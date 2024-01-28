# Diabetes Detection Models

This repository contains machine learning models for early detection of diabetes based on relevant features. Different models have been trained and evaluated for their performance.

## Models

### RandomForest Model (Before Hyperparameter Tuning - rf_model)

- **F1 Score:** 0.9984
- **Accuracy Score:** 0.9981
- **Confusion Matrix:** [[200   0] [  1 319]]
- **Cross Validation Score:** [0.9615, 0.9808, 0.9231, 1.0, 1.0]
- **Cross Validation Run Time:** 4.82 seconds
- **Mean Cross Validation:** 0.9769
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 1.0, 1.0]
  - **Recall:** [1.0, 0.9969, 0.0]
  - **Thresholds:** [0, 1]

### RandomForest Model (After Hyperparameter Tuning)

- **F1 Score:** 0.9671
- **Accuracy Score:** 0.9596
- **Confusion Matrix:** [[190  10] [ 11 309]]
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 0.9687, 1.0]
  - **Recall:** [1.0, 0.9656, 0.0]
  - **Thresholds:** [0, 1]

### GradientBoostingClassifier Model (Before Hyperparameter Tuning - gbc_model)

- **F1 Score:** 0.9969
- **Accuracy Score:** 0.9962
- **Confusion Matrix:** [[200   0] [  2 318]]
- **Cross Validation Score:** [0.9423, 0.9808, 0.9327, 0.9904, 0.9904]
- **Cross Validation Run Time:** 3.59 seconds
- **Mean Cross Validation:** 0.9673
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 1.0, 1.0]
  - **Recall:** [1.0, 0.9938, 0.0]
  - **Thresholds:** [0, 1]

### GradientBoostingClassifier Model (After Hyperparameter Tuning)

- **F1 Score:** 0.9969
- **Accuracy Score:** 0.9962
- **Confusion Matrix:** [[200   0] [  2 318]]
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 1.0, 1.0]
  - **Recall:** [1.0, 0.9938, 0.0]
  - **Thresholds:** [0, 1]

### XGBClassifier Model (Before Hyperparameter Tuning - xgb_model)

- **F1 Score:** 0.9953
- **Accuracy Score:** 0.9942
- **Confusion Matrix:** [[200   0] [  3 317]]
- **Cross Validation Score:** [0.9519, 0.9808, 0.9135, 0.9904, 1.0]
- **Cross Validation Run Time:** 2.10 seconds
- **Mean Cross Validation:** 0.9673
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 1.0, 1.0]
  - **Recall:** [1.0, 0.9906, 0.0]
  - **Thresholds:** [0, 1]

### XGBClassifier Model (After Hyperparameter Tuning)

- **F1 Score:** 0.9378
- **Accuracy Score:** 0.9212
- **Confusion Matrix:** [[170  30] [ 11 309]]
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 0.9115, 1.0]
  - **Recall:** [1.0, 0.9656, 0.0]
  - **Thresholds:** [0, 1]

### DecisionTree Model (After Hyperparameter Tuning)

- **F1 Score:** 0.9360
- **Accuracy Score:** 0.9212
- **Confusion Matrix:** [[179  21] [ 20 300]]
- **Precision-Recall Curve:**
  - **Precision:** [0.6154, 0.9346, 1.0]
  - **Recall:** [1.0, 0.9375, 0.0]
  - **Thresholds:** [0, 1]

## Conclusion

- The RandomForest model before hyperparameter tuning achieved an impressive F1 Score of 0.9984 and an accuracy of 99.81%, making it a strong candidate for detecting early signs of diabetes.
- After hyperparameter tuning, the RandomForest model maintained a high F1 Score of 0.9671 and an accuracy of 95.96%, showing robust performance.
- GradientBoostingClassifier models demonstrated excellent performance both before and after hyperparameter tuning, with F1 Scores of 0.9969 and high accuracies.
- The XGBClassifier model, while strong before tuning, experienced a decrease in performance after tuning, with an F1 Score of 0.9378.
- The DecisionTree model, after tuning, showed good performance with an F1 Score of 0.9360.

Overall, the RandomForest model (after tuning) and GradientBoostingClassifier models (both before and after tuning) appear to be the top performers for detecting diabetes at an early stage.

## Recommendations

- Based on the evaluation, it is recommended to deploy the tuned RandomForest and GradientBoostingClassifier models for real-world applications.
- Continuous monitoring and periodic retraining of the models with new data are essential for maintaining optimal performance.
- Collaboration with healthcare professionals to incorporate domain knowledge and additional relevant features could enhance model accuracy.
