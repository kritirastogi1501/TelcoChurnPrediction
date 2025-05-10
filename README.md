Telco Customer Churn Prediction

This project is a machine learning classification task aimed at predicting customer churn in the telecom industry. Using a dataset from Kaggle with over 7,000 customer records and 21 features, we explore patterns in customer behavior and use five popular classification models to build, evaluate, and tune a robust prediction system.

📁 Dataset Overview
- Source: [Kaggle Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)
- Format: CSV
- Rows: 7,043 customers
- Columns: 21 (features include customer demographics, service usage, billing info, and churn status)
Target Variable: `Churn` — whether a customer has left the service (`Yes` or `No`)

🛠️ Models Used
I trained and evaluated the following **classification algorithms**:
1. Logistic Regression
2. Support Vector Machine (SVM)
3. K-Nearest Neighbors (KNN)
4. Decision Tree
5. Random Forest
Each model is:
- Trained on the original dataset
- Evaluated using accuracy and a full classification report
- Hyperparameter-tuned using techniques like grid search or manual tuning
- Compared visually using bar plots

⚙️ Hyperparameter Tuning
To improve model performance, we tested various combinations of hyperparameters for each classifier. Plots are generated to show:
- Training Accuracy vs. Hyperparameters
- Testing Accuracy vs. Hyperparameters
  
📊 Visualizations
- Distribution plots for features like tenure, charges
- Count plots for categorical data and churn frequency
- Correlation heatmap
- Pairplots (or matplotlib equivalents) to observe feature interactions
- Bar chart comparing all model accuracies

🧠 Final Model Comparison
All five models are compared, and a bar plot summarizes their final test accuracies after tuning. This helps identify the **best-performing model**.

🎯 Interactive User Prediction
At the end of the notebook, we implemented a **user input system**:
- User enters values for all input features (e.g., contract type, tenure, charges)
- The **best-performing model** is selected automatically
- The model makes a churn prediction
- The result is displayed along with the model’s accuracy

🧰 Tech Stack
- Language: Python
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- Environment: Jupyter Notebook
