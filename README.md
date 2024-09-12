# 📞 Telecom Churn Prediction Case Study

**Predicting customer churn in the telecom industry with machine learning**

In this project, we dive into a real-world telecom dataset to predict customer churn, applying data science techniques to extract insights and build powerful predictive models. The outcome? A **93% accuracy** on the test set after model stacking! 🚀



## 🌟 Project Highlights
- **Churn Prediction**: Identifying customers at risk of leaving based on historical data.
- **Data Engineering**: Feature selection and deriving new columns using correlation and aggregation techniques.
- **Modeling Techniques**: Logistic Regression and Random Forests with model stacking.
- **Class Imbalance Handling**: Using SMOTE to balance churn/non-churn samples.
- **High Accuracy**: Achieving 93% accuracy on the test set through careful feature selection and model tuning.



## 📑 Workflow Breakdown

### 1. 🛠 Importing Libraries
We begin by importing all necessary Python libraries for data manipulation, visualization, and machine learning:
- **pandas**, **numpy** for data wrangling
- **matplotlib**, **seaborn** for data visualization
- **scikit-learn** for modeling and feature selection
- **SMOTE** for handling class imbalance

### 2. 📂 Getting Data from Kaggle API
We directly fetched the dataset using the **Kaggle API**, ensuring a smooth and reproducible workflow:

kaggle competitions download -c telecom-churn-case-study-hackathon-c-63

### 3. 🔍 Data Understanding
In this phase, we explored the dataset to understand key variables:
- Summary statistics, data types, and unique values.
- Distribution of the target variable (**Churn**), and spotting patterns in the data.

### 4. 📊 Selecting Key Columns & Deriving New Features
Leveraging:
- **Correlation analysis** to identify the most predictive features.
- **Aggregation techniques** to engineer new features, such as total recharge amounts, average call duration, and data usage.
- Dropped irrelevant columns like `customerID` and non-predictive date fields.

### 5. 🚧 Handling Missing Values
- Handled missing data using a combination of imputation strategies (mean, mode).
- Ensured no data leakage by only imputing based on the training set.

### 6. ✂️ Train-Test Split
The data was split into training and testing sets (80/20) to maintain generalizability and avoid overfitting:

### 7. 📈 Exploratory Data Analysis (EDA)
- Visualized feature distributions and correlations with the target.
- Handled **outliers** using techniques such as z-scores and IQR.
  
### 8. ⚖️ Feature Scaling
- Applied **StandardScaler** to normalize features and ensure uniform scaling across models:

### 9. 🔑 Finding Important Features
- Used **Recursive Feature Elimination (RFE)** and manual feature selection based on **Random Forest** and **PCA** results.
- Dropped less relevant features to streamline the model and prevent overfitting.

### 10. 🧠 Model Building & Stacking
- Built models using **Logistic Regression** and **Random Forest**.
- Applied **model stacking** for improved predictive performance:
  - Logistic Regression captured linear relationships.
  - Random Forest added non-linear predictive power.
Achieved **93% accuracy** on the test set after stacking!

### 11. 📝 Creating Submission File
Generated a final submission file by predicting churn probabilities on the test data, ready for Kaggle competition




## ⚙️ Technologies Used
- **Languages**: Python
- **Libraries**: pandas, numpy, scikit-learn, SMOTE, matplotlib, seaborn
- **Tools**: Kaggle API, Jupyter Notebooks



## 💡 Results & Learnings
- **93% accuracy** on the test set with stacked models.
- Discovered key churn drivers through feature importance from **Random Forest** and **PCA**.



## 🚀 Future Improvements
- Implement **boosting techniques** like XGBoost for potentially better performance.
- Apply regex filtering to automate the feature selection process and fine-tune the model further.

## 📜 Citation
www.kaggle.com/competitions/telecom-churn-case-study-hackathon-c-63/overview/$citation



## 📞 Contact
Feel free to reach out for any queries or discussions regarding this project:

LinkedIn: www.linkedin.com/in/shivani-iiitb
GitHub: https://github.com/Shivani3797
Email: bshivani572@gmail.com
If you have suggestions for improvements or want to collaborate on similar projects, I’d love to connect!
  


## 🤝 Connect
If you're interested in churn prediction, machine learning, or feature engineering, feel free to reach out or leave feedback on this project!



