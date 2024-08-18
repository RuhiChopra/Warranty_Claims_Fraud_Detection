# Warranty Claims Fraud Prediction

## Project Overview
The objective of this data science project is to predict the authenticity of warranty claims by analyzing various factors such as region, product category, claim value, and more. The dataset used for this project was sourced from Kaggle and consists of 358 rows and 21 columns.

## Data Dictionary

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| Unnamed: 0          | Index                                                                       |
| Region              | Region where the warranty claim was made                                    |
| State               | State where the warranty claim was made                                     |
| Area                | Area type (Urban/Rural) where the warranty claim was made                   |
| City                | City where the warranty claim was made                                      |
| Consumer_profile    | Profile of the consumer (Business/Personal)                                 |
| Product_category    | Product category (Household/Entertainment)                                  |
| Product_type        | Product type (AC/TV)                                                        |
| AC_1001_Issue       | Issue with AC component 1 (0 - No issue, 1 - Repair, 2 - Replacement)        |
| AC_1002_Issue       | Issue with AC component 2 (0 - No issue, 1 - Repair, 2 - Replacement)        |
| AC_1003_Issue       | Issue with AC component 3 (0 - No issue, 1 - Repair, 2 - Replacement)        |
| TV_2001_Issue       | Issue with TV component 1 (0 - No issue, 1 - Repair, 2 - Replacement)        |
| TV_2002_Issue       | Issue with TV component 2 (0 - No issue, 1 - Repair, 2 - Replacement)        |
| TV_2003_Issue       | Issue with TV component 3 (0 - No issue, 1 - Repair, 2 - Replacement)        |
| Claim_Value         | Value of the claim in INR                                                   |
| Service_Center      | Code of the service center where the claim was processed                     |
| Product_Age         | Age of the product in days                                                  |
| Purchased_from      | Source of purchase (Dealer, Manufacturer, Internet)                         |
| Call_details        | Duration of the customer care call                                          |
| Purpose             | Purpose of the customer care call                                           |
| Fraud               | Fraudulent (1) or Genuine (0) claim conclusion                              |

## Conclusion
Key insights from the exploratory data analysis:

- **Regional Trends**: Warranty claims are most frequent in the southern region of India, particularly in Andhra Pradesh and Tamil Nadu.
- **Urban vs Rural**: Fraudulent claims are more common in urban regions such as Hyderabad and Chennai.
- **Product Analysis**: TVs have higher warranty claims, especially when purchased for personal use. Fraudulent claims for ACs occur even when there are no issues with the AC parts, whereas fraudulent TV claims can occur with or without issues in the TV parts.
- **Purchase Source**: Fraudulent claims are more frequent when purchases are made directly through the manufacturer.
- **Claim Value**: Fraudulent claims tend to have higher claim values compared to genuine claims.
- **Service Center Analysis**: Service center 13 had the highest number of fraudulent claims despite handling fewer total warranty claims.
- **Call Duration**: Fraudulent claims are more likely when the customer care call duration is less than 3-4 minutes.

## Modeling and Results

Machine learning models employed:

- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Logistic Regression**

**Performance**:
- Achieved accuracy levels of 91-92% in predicting fraudulent claims.
- Models showed excellent accuracy but lower recall scores for fraudulent claims due to the limited number of fraudulent instances and small dataset size. This can be improved by expanding the dataset.

## Future Work
This project demonstrates significant potential for identifying and preventing warranty claims fraud, contributing to resource savings and enhancing the efficiency of warranty claim processing. Future work should focus on increasing the dataset size to improve model robustness and recall scores for fraudulent claims.

