# Customer-Churn-Prediction
This project predicts customer churn for a telcom company.
The data includes customer details, services, and billing info.

Goal -> find what causes churn and build models to **reduce customer loss**.

### <u>PROJECT WORKFLOW</u>

#### 1. Data Cleaning
 - Dropped useless columns (Customer ID, Country, etc).
 - Filled missing values:
      - offer -> "No Offer"
      - Internet Type -> "No Internet"
 - Changed **Churn Label** -> Yes = 1, No = 0.
 - Fixed *Total Charges* -> made numeric, filled missing with median.

#### 2. EDA (Exploratory Data Analysis)
 - **Churn Distribution** -> more customers stayed than left.
 - **Gender & Age** -> churn not linked to gender, younger churn a bit more.
 - **Contract** -> month-to-month churns most
 - **Internet Service** -> fiber optic churns more.
 - **Monthly Charges** -> higher charges = more churn.
 - **Heatmap -> tenure and contract are strong factores.

#### 3. Data Preprocessing
 - Encoded target column.
 - One-hot encoding for categories.
 - Train/test split -> 80/20.
 - Standardized with StandardScaler.

#### 4. Models Used
 -**Logistic Regression**
 -**Random Forest**
 -**Gradient Boosting**
Metrics -> Accuracy, Precision, Recall, F1, ROC-AUC.

#### 5. Results
 - Gradient Boosting : best model.
 - Random Forest : good.
 - Logistic Regression : less accurate.
We plotted:
 - ROC Curve for all models.
 - Feature Importance (top 15 factors).

### INSIGHTS
 1. **Month-to-month contracts** = high churn.
 2. **High monthly charges + short time with company** = high churn.
 3. **Fiber optic users** churn more than DSL.
 4. Seniors and customers with **no dependents** churn more.
 5. Discounts and loyalty programs can help.

### CONCLUSION
 - Best model ->**Gradient Boosting**.
 - To reduce churn, businesses should:
     - Push **long-term contracts.
     - Give **discounts to high-bill users**.
     - Offer **loyalty rewards in first year**
  
### TOOLS USED
 - Python
 - Pandas, NumPy
 - Seaborn, Matplotlib
 - Scikit-learn
 - Random Forest, Gradient Boosting, Logistic Rregression
