# Credit Risk Analysis
The objective of this analysis was to identify the best machine learning model that would predict if a loan applicant is high risk.  A number of machine learning algorithms were tested to find which one performed the best.  

## Results

### Random Oversampling
* Balanced Accuracy: 0.63
* Precision: 0.01
* Recall: 0.66
![random_oversampling_balanced_accuracy](random_oversampling_balanced_accuracy.png)
![random_oversampling_classification_report](random_oversampling_classification_report.png)
### SMOTE Oversampling
* Balanced Accuracy: 0.66
* Precision: 0.01
* Recall: 0.62
![SMOTE_balanced_accuracy](SMOTE_balanced_accuracy.png)
![SMOTE_classification_report](SMOTE_classification_report.png)
### Under Sampling
* Balanced Accuracy: 0.66
* Precision: 0.01
* Recall: 0.69
![undersampling_balanced_accuracy](undersampling_balanced_accuracy.png)
![undersampling_classification_report](undersampling_classification_report.png)
### Combination Sampling
* Balanced Accuracy: 0.54
* Precision: 0.01
* Recall: 0.79
![combination_sampling_balanced_accuracy](combination_sampling_balanced_accuracy.png)
![combination_sampling_classification_report](combination_sampling_classification_report.png)
### Balanced Random Forest Classifier
* Balanced Accuracy: 0.77
* Precision: 0.03
* Recall: 0.64
![balanced_random_forest_balanced_accuracy](balanced_random_forest_balanced_accuracy.png)
![balanced_random_forest_classification_report](balanced_random_forest_classification_report.png)
### Easy Ensemble AdaBoost Classifier
* Balanced Accuracy: 0.91
* Precision: 0.05
* Recall: 0.93
![easy_ensemble_balanced_accuracy](easy_ensemble_balanced_accuracy.png)
![easy_ensemble_classification_report](easy_ensemble_classification_report.png)

## Summary
The Easy Ensemble AdaBoost model performed the best out of all of the options tested.  It scored the best across balanced accuracy, precision, and recall.  However, the precision scores are still very low.  Boosting did help improve the precision scores by a signicant amount, but there is only so much that process can help with such an imbalanced data set.  If the priority is to be conservative, then I would recommend using the Easy Ensemble AdaBoost model.  You would get a high number of false positives, but you would reduce the amount of loans given to high risk borrowers.  
