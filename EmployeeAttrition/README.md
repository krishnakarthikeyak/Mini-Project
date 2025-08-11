# Mini-Project


Project Title: 

Employee Attrition Prediction Using Machine Learning  


Project Role: 

Contributor (Project Idea Originator)


Project Type: 

Group Project (3 members) 


Tools & Techniques: 

CatBoost, XGBoost Regressor, Random Forest, SMOTE, Hyperparameter Tuning, IBM-HR Dataset.


Description:

Enhanced a base model project that analyzed employee attrition using machine learning algorithms. 
Improved the performance by balancing the dataset with SMOTE and introducing new algorithms, including CatBoost and XGBoost Regressor. 
Further optimized the best performing algorithm through hyperparameter tuning. 
This project aimed to help organizations mitigate employee attrition by identifying at-risk employees and suggesting actionable strategies such as improving facilities, offering better pay, and enhancing work-life balance.


Project Overview:

This project is based on the algorithms explored in the base paper, which included Random Forest, Support Vector Machines (SVM), Logistic Regression, among others. The base paper concluded that Random Forest was the best-performing algorithm. However, it also identified that the dataset used was unbalanced, potentially affecting the model's performance.


Our Approach

1. Data Preprocessing: Balancing the Dataset
To address the issue of imbalance in the dataset, we applied **SMOTE (Synthetic Minority Over-sampling Technique)**. SMOTE is an over-sampling method that creates synthetic samples from the minority class, thereby balancing the dataset.

2. Algorithm Evaluation
After balancing the dataset, we re-evaluated several machine learning algorithms, including:
- **Random Forest** (as a benchmark from the base paper)
- **XGBoost**
- **CatBoost**

Our experiments demonstrated that both XGBoost and CatBoost outperformed Random Forest, providing better accuracy and generalization.

3. Hyperparameter Tuning
Given that XGBoost emerged as the best-performing algorithm, we performed hyperparameter tuning to further optimize its performance. This step involved fine-tuning parameters like learning rate, max depth, and the number of estimators to achieve the best possible results.


Conclusion:

Through this work, we have shown that, by balancing the dataset and exploring more advanced algorithms like XGBoost and CatBoost, we can significantly improve the model's performance over the Random Forest benchmark.

