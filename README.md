# Age-Prediction-from-MRI-Images
In this project, the goal is to predict patient age using condensed tabular features extracted from brain MRI images, rather than raw image data.

The problem is formulated as a supervised regression task, where each sample consists of MRI-derived features and a corresponding chronological age.
The dataset contains missing values, outliers, and high-dimensional features, making robust preprocessing essential for good performance.

To address these challenges, a complete data preprocessing pipeline was developed, including missing value imputation, outlier handling, feature scaling, and feature selection.
Careful fine-tuning of this pipeline proved critical to improving model accuracy and generalization.

After identifying the optimal preprocessing strategy, an XGBoost regressor was trained, as it represents a state-of-the-art approach for tabular data.
The model was optimized by minimizing the Mean Squared Error (MSE) loss to achieve accurate age predictions.
