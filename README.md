# Telecom Customer Churn Prediction

## Project Overview
This project focuses on predicting customer churn in the telecom industry using machine learning techniques. Customer churn refers to customers leaving the service. The aim of this project is to identify customers who are likely to churn so that businesses can take steps to retain them.

The project uses a real-world telecom dataset and applies data preprocessing, exploratory data analysis, and multiple machine learning models to compare performance and identify the most effective approach.


## Dataset
- **Source:** Kaggle – Telecom Customer Churn Dataset  
- **Target Variable:** Churn  
  - `1` = Yes (Customer churned)  
  - `0` = No (Customer did not churn)

The dataset contains customer demographic details, service usage information, and billing-related features.


## Data Preprocessing
- Categorical variables were converted into numerical values using label encoding and one-hot encoding.
- The dataset was split into training and testing sets using an 80/20 split.
- Class imbalance was handled using SMOTE, applied only to the training data.


## Exploratory Data Analysis (EDA)
Exploratory analysis was performed to understand patterns in the data. Visualisations were used to study the relationship between customer churn and features such as monthly charges, contract type, and tenure.


## Models Used
- Logistic Regression (baseline model)
- Random Forest
- XGBoost


## Model Evaluation
Models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  

These metrics were chosen to ensure fair evaluation for imbalanced churn data.


## Model Optimization
Hyperparameter tuning was performed using GridSearchCV. After tuning:
- Logistic Regression achieved the highest accuracy.
- Random Forest showed balanced performance.
- XGBoost achieved the highest recall for churned customers.


## Key Findings
- Customers with higher monthly charges are more likely to churn.
- Ensemble models performed better than simple models.
- Random Forest provided the best balance between identifying churners and avoiding false predictions.


## Limitations
- SMOTE generates synthetic data, which may not fully reflect real customer behaviour.
- The test dataset remains imbalanced.
- Some customer behaviour features were not available.


## Future Work
- Use the model for real-time churn prediction.
- Add more customer behaviour features.
- Improve model explainability using SHAP.
- Apply the approach to other industries such as banking or insurance.


## Tools and Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  
- Imbalanced-learn (SMOTE)


## Conclusion
This project shows that machine learning models can effectively predict customer churn in the telecom sector. Proper data preprocessing, class balancing, and model tuning play an important role in improving prediction performance.


## License
This project is licensed under the MIT License.


## Author
**Deepak Raj**  
GitHub: https://github.com/deepakraj-04
