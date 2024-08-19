# Credit-Risk-Analysis-Using-Machine-Learning

This project focuses on analyzing and predicting credit risk using machine learning models. The primary goal is to develop a system that accurately predicts loan default probabilities and classifies applicants into appropriate risk categories (Low Risk or High Risk). This project leverages various data preprocessing techniques, machine learning models, and performance evaluation methods to ensure a robust and reliable credit risk prediction system.

Key Features:
Data Preprocessing:

Handling Missing Values: Missing values in critical features such as person_emp_length and loan_int_rate are imputed using the median to preserve the dataset's integrity.
Outlier Detection and Removal: Outliers in numerical features are detected and removed using the Interquartile Range (IQR) method to enhance model performance.
Feature Encoding: Ordinal and nominal categorical features are encoded using Label Encoding and One-Hot Encoding, respectively, ensuring that all features are numeric and suitable for model training.
Feature Scaling: Numerical features are standardized using StandardScaler to ensure uniformity across all features, improving model accuracy and convergence.
Class Imbalance Handling:

The dataset's inherent class imbalance is addressed using the SMOTE (Synthetic Minority Over-sampling Technique) to balance the target classes, ensuring the model does not favor any particular class.
Model Training and Evaluation:

Machine Learning Models: The project utilizes Logistic Regression, Decision Tree, and Random Forest classifiers. The models are trained and evaluated on the resampled dataset.
Model Evaluation Metrics: Comprehensive evaluation metrics, including accuracy, precision, recall, F1 score, and ROC-AUC, are calculated to assess each model's performance. The Random Forest model emerged as the best-performing model with the highest accuracy and F1 score.
Precision-Recall Curves: Precision-Recall curves are plotted for each model to visualize their performance, particularly in handling imbalanced data.
Prediction Functionality:

A prediction function is developed to integrate the trained Random Forest model into a real-world application. The function takes input features, preprocesses them similarly to the training data, and outputs a prediction with the associated risk category (Low Risk or High Risk).
Model Deployment:

The best-performing model (Random Forest) is saved using joblib for easy deployment. The project includes a script to load the model and make predictions on new input data, ensuring the system is ready for production use.
Visualization and Correlation Analysis:

The project includes visualizations of feature distributions before and after outlier handling and a correlation matrix to understand relationships between features, aiding in feature selection and model interpretation.
Conclusion:
This project successfully implements a comprehensive credit risk analysis system using machine learning. The use of advanced data preprocessing techniques, model evaluation, and a robust prediction function ensures the model's effectiveness in predicting loan default probabilities and classifying credit risk. The project is structured for scalability and ease of deployment, making it suitable for real-world applications in the financial industry.

