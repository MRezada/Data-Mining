 Breast Cancer Diagnosis Using Data Mining
This project aims to predict the type of breast tumor (benign or malignant) using medical features and data mining algorithms. The data includes various physical and statistical characteristics of the tumor, based on the worst recorded sample per patient.

Objective
To classify tumors as malignant (1) or benign (0) using relevant tumor features.

Independent Variables (Features)
radius_worst: Radius of the largest tumor sample

concave_points_worst: Number of severe concave points along the tumor edge

area_worst: Area of the worst tumor sample

texture_worst: Texture of the worst tumor sample

perimeter_worst: Perimeter of the largest tumor sample

Logistic Regression Analysis
Significant predictors based on p-value < 0.05:

concave_points_worst: A strong indicator—higher values sharply increase the likelihood of malignancy.

area_worst: Larger tumor areas are more likely to be malignant.

texture_worst: Irregular textures are associated with malignancy.

Decision Tree
The decision tree model uses thresholds to classify tumors. For example:

If radius_worst < 17, and concave_points_worst < 14, and texture_worst < 26 → most likely benign

Otherwise → likely malignant

Random Forest - Feature Importance
Based on accuracy reduction and Gini impurity:

concave_points_worst

area_worst

perimeter_worst

These features contribute most to model performance and decision clarity.

Model Evaluation
Confusion Matrix (Random Forest):
Benign detection accuracy: 97.2%

Malignant detection accuracy: 93.9%

SVM Model Performance:
Overall accuracy: ~94.6%

Sensitivity (Recall): 91.6%

Specificity: 97%

Precision (PPV): 94.8%

Negative Predictive Value (NPV): 95.1%

Conclusion
Data mining models like Logistic Regression, Decision Tree, Random Forest, and SVM have successfully classified tumor types with high accuracy. Features such as concave_points_worst and area_worst play a crucial role in predictive power.

