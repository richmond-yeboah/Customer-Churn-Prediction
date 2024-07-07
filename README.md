## Table of Content
- [Project Description](#project-description)
- [Installation](#installation)
- [Dataset and source](#dataset-and-source)
- [Data Preprocessing](#data-preprocessing)
- [Model Building and Evaluation](#model-building-and-evaluation)
- [Recommendations](#recommendations)
- [Power BI Dashboard and Insights](#power-bi-dashboard-and-insights)
- [Contact Information](#contact-information)



## Project Description

This is a live project that dives into the customer data of a telco company to unveil insights and hidden patterns about customers and what might be their reasons for churning so that the company can come up with customer retention strtagies. Also, an ML model will be built to help make churn predictions that can help the company tailor solutions to customers before they churn.

The success criteria of this project lies in building a highly accurate and interpretable machine learning model. This will require carefully chosen data features, effective model selection, and rigorous evaluation techniques. Ultimately, this project aims to equip companies with a powerful tool to combat customer churn and achieve sustainable growth.


## Installation

This project requires that you have a Python 3.9 or later version installed on your local machine. The modules and packages needed to complete this project are all contained in the requirements.txt file. Run this command in your terminal to get started on the project.


## Dataset and source

The datasets for this project were sourced from GitHub, Microsoft SQL Server, and a CSV file from Onedrive. The columns in the dataset and the values contained in them are provided below for data understanding.

| Attribute          | Description                                                    |
|--------------------|----------------------------------------------------------------|
| Gender             | Whether the customer is a male or a female                     |
| SeniorCitizen      | Whether a customer is a senior citizen or not                  |
| Partner            | Whether the customer has a partner or not (Yes, No)            |
| Dependents         | Whether the customer has dependents or not (Yes, No)           |
| Tenure             | Number of months the customer has stayed with the company      |
| PhoneService       | Whether the customer has a phone service or not (Yes, No)      |
| MultipleLines      | Whether the customer has multiple lines or not                 |
| InternetService    | Customer's internet service provider (DSL, Fiber Optic, No)    |
| OnlineSecurity     | Whether the customer has online security or not (Yes, No, No Internet) |
| OnlineBackup       | Whether the customer has online backup or not (Yes, No, No Internet) |
| DeviceProtection   | Whether the customer has device protection or not (Yes, No, No internet service) |
| TechSupport        | Whether the customer has tech support or not (Yes, No, No internet) |
| StreamingTV        | Whether the customer has streaming TV or not (Yes, No, No internet service) |
| StreamingMovies    | Whether the customer has streaming movies or not (Yes, No, No Internet service) |
| Contract           | The contract term of the customer (Month-to-Month, One year, Two year) |
| PaperlessBilling   | Whether the customer has paperless billing or not (Yes, No)    |
| PaymentMethod      | The customer's payment method (Electronic check, mailed check, Bank transfer(automatic), Credit card(automatic)) |
| MonthlyCharges     | The amount charged to the customer monthly                     |
| TotalCharges       | The total amount charged to the customer                       |
| Churn              | Whether the customer churned or not (Yes or No)                |


## Data Preprocessing
The dataset that was gathered had inconsistencies like null values, and wrong data types in certain columns, which had to be corrected. The null values were imputed using Simple Imputer and the data types for columns with wrong data types were corrected.

The necessary corrections that were to be made were put into a pipeline to ensure that these same processes were used when new datasets were provided. The categorical columns in the dataset were all changed to numerical values for the machine-learning model to learn efficiently using OneHot Encoder and Label Encoder.


## Model Building and Evaluation
Two datasets out of the three that were sourced from multiple places were concatenated and divided into features and target variables, after which it was split into train and evaluation sets with a percentage of 80% for training and evaluation for the remaining. The goal of this project is to build a robust machine-learning model hence, five models namely, RandomForest, DecisionTree, GradientBoosting, and SupportVector classifiers were trained.

The imbalanced nature of our target column called for a balancing of the dataset and this was done using both RandomSampler and SMOTE and it was seen that the latter performed better. Feature selection was implemented to improve the performance of the model, and also some hyperparameter tuning processes using RandomizedSearchCV.

The model's performance was assessed using the f1-score metric and the AUC-ROC curve. The f1-score blends precision and recall using their harmonic mean which means maximizing for the f1-score implies simultaneously maximizing for both precision and recall.

The AUC-ROC curve visually summarizes a classifier's ability to distinguish between classes across all thresholds, with a higher AUC indicating better separation (AUC = Area Under the ROC Curve). A graph for the ROC curve for all the models was plotted with their respective auc-score to help assess how the model is performing.

## Recommendations
The telco company should look to implement customer retention strategies tailored to addressing the pain points of customers that has been predicted to churn in the near future.

## Power BI Dashboard and Insights

![alt text](<PBI dashboard.png>)

- Percentage of customers that are males are 50.7% while Females constitute 49.3% of the total customers. Therefore male customers are slightly more than female customers according to the data.

- The average monthly charge for customers is 65.09 units.

- The number of customers that churned was 1,336 while 3,706 didn’t churn.

- A churn rate of 26.5% signifies a significant customer loss for the telco company, By addressing a 26.5% churn rate effectively, companies can minimize customer losses, improve customer lifetime value, and ensure sustainable growth.

- The churn rate by tenure visualization shows a decrease in churn rate as the tenure increases. Obviously, customers that have spent a long time with the telco company are customers that we can say are satisfied with the services of the company and, therefore, are less likely to join another telco company and leave the current one.

- Customers with a month-to-month contract have higher churn rate (43%) as compared to customer on longer contracts. Customers with such contracts might not have plans of staying with the company for long and might be new customers looking for short-term services therefore can’t risk signing longer contracts.

- Customers with partners or married customers have way less churn rate (20%) as compared to customers with no partner or single customers(33%).


check out the Power BI dashboard [here](https://app.powerbi.com/view?r=eyJrIjoiZjBlMDQwZDktODlhOS00ZDZjLTk1ZTUtNTk2OTUzNTNiMDQyIiwidCI6IjFjZTU4MjFjLTE5NDItNDczMy1hNmRjLTBmYzNhODJiNzRkYiJ9).

Also check out the project article [here](https://medium.com/@richmondyeboah299/telco-customer-churn-prediction-0fdb61ed68f9).


## Contact Information
- my email : richmondyeboah299@gmail.com

- my linkedin : www.linkedin.com/in/richmond-yeboah-