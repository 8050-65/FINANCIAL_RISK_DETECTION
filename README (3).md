# Financial Risk Detection
This project aims to leverage Exploratory Data Analysis (EDA)
and machine learning to conduct risk analysis for loan default
prediction in the context of a consumer finance company. By
analyzing historical loan application data, we will identify patterns
and factors that indicate whether a client is likely to default on their
loan payments. This analysis will assist the company in minimizing
financial losses while ensuring that creditworthy applicants are not
unfairly rejected.
# Tools Used:
* Python
* Pandas(Data Cleaning)
* Scikit-learn(Encoding, Scaling, Model building, Model evaluation)
* Matplotlib, Seaborn(Visualizations, EDA)
# Dataset
The dataset has 2 files.
  * Application Data
  * Previous Application
The Application data has many demographic columns, income details, type of loans, and the Target column(0 - defaulter, 1- Repayer)
The previous application has details of the users previous loan applications, status of application and reasons for rejection etc.
# Data Cleaning
The Huge dataset has numerous null values in different columns. The null values were filled with mean/median/mode values after the thorough analysis of different columns. 
The negative values and outliers in the data were handling accordingly.
The same methods were followed to clean and preprocess the Previous Application data set.
# Exploratory Data Analysis
EDA of both datasets were peformed separately and many meaningful insights were made.
# Model Building
* The datasets were then merged together for model building.
* The dataset was split with 'TARGET' column being the target variable.
* The important columns(top15) were selecting by feature selection method(chi2)
* As the target column was imbalanced, SMOTE technique was used for Oversampling
* The values in the numerical columns were too huge , hence the values were scaled using Satndard scaler
* As the Target is a categorical column,different classification algorithms were used to make the predictions.
* Finally Decision Tree was selected as the ideal model based on the Evaluation metrics.
* The model was then saved as a pickle file for making future predictions.
