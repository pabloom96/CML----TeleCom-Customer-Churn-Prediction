# CML----TeleCom-Customer-Churn-Prediction

**SUMMARY:**

Processed and visualized a TeleCom customer database to analyze behavioral patterns and trends. Built a Machine Learning model that predicts customer churn or retention, highlighting the most influential features driving churn behavior.

**Definition of the problem:**

The telecommunications operator Interconnect aims to forecast its customer churn rate. If a user is identified as likely to leave, they will be offered promotional codes and special plan options. The Interconnect marketing team has collected personal data from its customers, including information about their plans and contracts.

The dataset contains information about customers of a telecommunications company and is distributed across four tables related by customerID:

* Contract (7,043 records): Contractual and billing information, including contract start and end dates, contract type (monthly, yearly, biennial), payment method, paperless billing, and monthly and total charges.
* Personal (7,043 records): Customer demographic data, such as gender, senior status, partnership status, and dependents.
* Phone (6,361 records): Phone service details, including whether the customer has multiple phone lines.
* Internet (5,517 records): Internet service details, such as connection type (DSL or fiber optic) and additional services (online security, online backup, device protection, technical support, TV and movie streaming).

The difference in record counts between tables suggests that not all customers subscribe to all services (phone and internet).

Target feature: The 'EndDate' column equals 'No'.
Main metric: AUC-ROC.

* Language: Python 3.10
* Environment: Jupyter Notebook
  * Main Libraries:
    * Joblib (model exportation)
    * Pandas (data processing)
    * Math / Numpy (numerical operations)
    * Matplotlib / seaborn (data visualization)
    * SHAP (feature importance visualitation)
    * Pycaret (algorithm suggestion)
    * Scikit-learn (modeling, validation and evaluation)
    * XGBoost, LightGBM, CatBoost (gradient boosting algorithms) 

      
**How to Run:**

1. Clone this repository.
2. Open the .ipynb file in Jupyter Notebook or VS Code.
3. Run the cells in order.

Due the ammount of data, the use of tools like GridSearch and the use of best hyperparameters on gradient boosting algorithms, the computational resources needed to train the models are high, so the notebook uses joblib to save those models and export them as pkl files. Those files are available on the dashboard to make it easier to run.
