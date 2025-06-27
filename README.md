# Task-4
Breast Cancer Classification using Logistic Regression:
This project implements a binary classification model using Logistic Regression on the Breast Cancer Wisconsin dataset from Kaggle. The primary objective is to predict whether a tumor is Malignant (1) or Benign (0) based on various medical measurements.
The dataset contains 569 records of tumor samples, each with 30 numerical features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. The target variable is the diagnosis (M = malignant, B = benign), which was encoded as 1 and 0 respectively.

Workflow:

1) Data Preprocessing:
Removed irrelevant columns like id and Unnamed: 32.
Encoded categorical diagnosis labels into binary values.
Handled missing values and separated features from the target.
Standardized the data using StandardScaler.

2) Model Training:
Trained a Logistic Regression model with various configurations:
Basic model with L2 regularization.
L1 regularized model using the liblinear solver.
Model with class_weight='balanced' to handle potential imbalance.
Evaluated model robustness using 5-fold cross-validation.

3) Model Evaluation:
Evaluated using accuracy, precision, recall, F1 score, and ROC-AUC.
Visualized the confusion matrix using a heatmap.
Plotted ROC curve and computed AUC score.
Created a Precision-Recall vs Threshold plot to analyze decision threshold impact.

4) Threshold Tuning and Sigmoid Function:
Explained the role of the sigmoid function in logistic regression.
Demonstrated the effect of custom thresholds on prediction performance.
Computed and visualized the optimal threshold based on F1 score.

5) Feature Importance:
Interpreted model coefficients to identify top contributing features.
Visualized top 10 influential features using a horizontal bar chart.

Innovations and Add-ons: 
1) Manual and visual threshold tuning to optimize recall in medical diagnosis.
2) Cross-validation metrics boxplot to validate model stability.
3) Custom prediction function for real-time prediction testing.
4) Visual explanation of the sigmoid activation curve for better interpretability.

   Conclusion: 
The logistic regression model performed effectively on the dataset, achieving high recall and AUC, which is critical in healthcare applications where false negatives must be minimized. The project demonstrates how a simple and interpretable model like logistic regression can be enhanced through thoughtful evaluation, threshold tuning, and visualization techniques.

