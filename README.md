# FruitClassification
## Introduction 
This report summarizes the analysis and modelling of a fruit classification dataset containing attributes like size, weight, price, shape , color, taste, and fruit name. The goal was to predict fruit name. The goal was to predict fruit types based on these characteristics.
### Data Overview
- Dataset: Fruit classification data with 7 features and a target variable (fruit_name).
- Shape: (1000, 8) - 1000 samples, 8 columns.
- Features:
    - Numerical: size (cm), weight (g), avg_price (₹)
    - Categorical: shape, color, taste, fruit_name

### Exploratory Data Analysis (EDA)
1. Duplicates: 246 duplicates found; retained as they represented valid data points.
2. Correlations:
    - Moderate positive correlation between size (cm) and weight (g) (0.65).
    - Weak correlations between other numerical features.
3. Visualizations:
    - Scatter plot: size (cm) vs weight (g) showed a positive trend.
    - Correlation heatmap highlighted relationships between numerical features.

### Data Preprocessing
- Encoded categorical variables (shape, color, taste, fruit_name) using LabelEncoder.
- Split data into training (80%) and testing (20%) sets.

### Modeling
1. K-Nearest Neighbors (KNN):
    - Accuracy: 98.10%
2. Support Vector Machine (SVM):
    - Accuracy: 71.25%
3. Random Forest:
    - Accuracy: 96.24%
4. Decision Tree:
    - Accuracy: 100.00%
5. Logistic Regression:
    - Accuracy: 99.85%
6. Naive Bayes:
    - Accuracy: 100.00%
7. XGBoost:
    - Accuracy: 89.5% (previously reported; might need re-checking)

### Evaluation Metrics
- Accuracy: Decision Tree and Naive Bayes achieved perfect scores (100%).
- Classification Report: High precision, recall, F1-score for most classes.
- Confusion Matrix: Minimal to no misclassifications with top models.

### Key Findings
- Decision Tree and Naive Bayes emerged as top performers, capturing patterns effectively.
- KNN and Logistic Regression also showed strong performance.
- SVM had relatively lower accuracy, suggesting data might not be linearly separable.

### Recommendations
1. Model Selection: Consider Decision Tree or Naive Bayes for simplicity and performance.
2. Hyperparameter Tuning: Further optimize models for potential gains.
3. Deployment: Deploy the chosen model for real-world fruit classification.

### Tools & Libraries
- Python: Pandas, NumPy, Scikit-learn, XGBoost
- Visualization: Matplotlib, Seaborn

### Conclusion
The Decision Tree and Naive Bayes models demonstrated excellent potential for classifying fruits based on given attributes.

## Appendix
### Model Performance Comparison
| Model | Accuracy |
| ----- | -------- | 
| KNN | 98.10% |
| SVM | 71.25% |
| Random Forest | 96.24% |
| Decision Tree | *100.00%* |
| Logistic Regression | 99.85% |
| Naive Bayes | *100.00%* |
| XGBoost | 89.5% |
