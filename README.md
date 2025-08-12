Loan Defaulter Classification

📌 Project Overview

This project aims to classify loan defaulters and non-defaulters to support financial institutions in making informed lending decisions.
The workflow starts from custom data collection using Selenium web scraping, followed by data cleaning, exploratory data analysis (EDA), and machine learning modeling using a Random Forest Classifier.
        
🧹 Data Cleaning

    Removed duplicate records.

    Handled missing values appropriately.

    Converted data types for modeling readiness.

📈 Exploratory Data Analysis (EDA) & Visualization

Performed:

    Univariate analysis (distribution of individual features)

    Bivariate analysis (relationship between features and target variable)

    Correlation analysis (heatmaps for numeric features)

🤖 Model Development

    Algorithm Used: Random Forest Classifier inside a preprocessing pipeline.

    Feature Processing:

        Continuous features were scaled.

        Categorical features were one-hot encoded.

        Train-Test Split: 80% training, 20% testing.

📊 Model Performance

    Accuracy: 94.03%

    Precision/Recall/F1:

        Class 0 (Non-defaulters): Excellent performance, recall = 1.00

        Class 1 (Defaulters): Lower recall = 0.30 (model misses some actual defaulters)

Classification Report :
📌 Key Notes

    The model is highly accurate in predicting non-defaulters but needs improvement in detecting defaulters.

    Likely class imbalance issue in the dataset.

    Suggested improvements:

        Apply SMOTE / oversampling.

        Test alternative algorithms like XGBoost, LightGBM.

        Enhance feature engineering.

🛠 Tech Stack

    Languages & Tools: Python, Jupyter Notebook

    Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

    ML Algorithm: Random Forest Classifier

🚀 How to Run

    Open the notebook in Jupyter.

    Install required libraries listed in requirements.txt.

    Execute the notebook step-by-step to reproduce results.
