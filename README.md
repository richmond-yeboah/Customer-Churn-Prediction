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


