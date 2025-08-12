Loan Defaulter Classification
📌 Project Overview

This project aims to classify loan defaulters and non-defaulters to support financial institutions in making informed lending decisions.
The workflow starts from custom data collection using Selenium web scraping, followed by data cleaning, exploratory data analysis (EDA), and machine learning modeling using a Random Forest Classifier.
📊 Data Collection

    Source: Cars24

    Method: Automated scraping using Selenium to collect real car listing details.

    Stored Format: CSV file containing columns like:

        Name

        Model

        Company

        Year

        Fuel Type

        KM Driven

        Transmission Type

        Price (in Lakh)

        Location

Sample Records:
Name	Model	Company	Year	Fuel Type	KM Driven	Transmission	Price	Location
Hyundai Creta SX PLUS AT 1.6 PETROL	Creta SX PLUS AT 1.6 PETROL	Hyundai	2017	PETROL	98493	Automatic	973000	Bangalore
Renault Kwid 1.0 MARVEL IRON MAN EDITION AMT	Kwid 1.0 MARVEL IRON MAN EDITION AMT	Renault	2018	PETROL	19178	Automatic	407000	Bangalore
🧹 Data Cleaning

    Removed duplicate records.

    Detected and eliminated outliers in features like Price and KM Driven.

    Handled missing values appropriately.

    Converted data types for modeling readiness.

📈 Exploratory Data Analysis (EDA) & Visualization

Performed:

    Univariate analysis (distribution of individual features)

    Bivariate analysis (relationship between features and target variable)

    Correlation analysis (heatmaps for numeric features)

Key Observations:

    Higher car prices generally correlated with a lower likelihood of default.

    Certain locations and models were more common among customers.

    Fuel type and transmission showed patterns that may influence default risk.

EDA Visuals:
(Insert screenshots here)

    Distribution of Price

    Countplot of Fuel Type vs Target

    Heatmap of numerical feature correlations

    Boxplot showing KM Driven by Target

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

Classification Report Visual:
(Insert screenshot here)
📌 Key Notes

    The model is highly accurate in predicting non-defaulters but needs improvement in detecting defaulters.

    Likely class imbalance issue in the dataset.

    Suggested improvements:

        Apply SMOTE / oversampling.

        Test alternative algorithms like XGBoost, LightGBM.

        Enhance feature engineering.

🛠 Tech Stack

    Languages & Tools: Python, Jupyter Notebook

    Libraries: Selenium, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

    ML Algorithm: Random Forest Classifier

🚀 How to Run

    Open the notebook in Jupyter.

    Install required libraries listed in requirements.txt.

    Execute the notebook step-by-step to reproduce results.
