# GT-Bank-Customer-Churn-Analysis

## Project Overview

This project analyzes customer churn data for GT Bank to understand the factors associated with customers leaving the bank. The analysis examines customer demographics, location, account characteristics, balance levels, tenure, credit card ownership, and membership activity.

Using **Microsoft Excel**, the dataset was cleaned, transformed, analyzed using PivotTables, and visualized through charts and an interactive dashboard. The analysis provides insights that can help identify customer groups with higher churn and support customer retention strategies.

---

## Project Objective

The main objective of this project is to analyze customer churn patterns and identify the characteristics and behaviors associated with customer attrition.

### Specific Objectives

* Determine the overall customer churn rate.
* Analyze churn across different age groups and genders.
* Compare churn across customer locations.
* Examine the relationship between customer lifetime and churn.
* Analyze churn by balance groups.
* Investigate the relationship between credit card ownership and churn.
* Compare churn between active and inactive members.
* Identify customer segments that may require targeted retention efforts.
* Develop a dashboard for communicating key findings.

---

## Business Problem

Customer churn can reduce revenue, increase customer acquisition costs, and weaken long-term customer relationships. GT Bank needs to understand **which types of customers are more likely to leave and which customer characteristics are associated with higher churn**.

The key business questions addressed in this project include:

1. What percentage of customers have churned?
2. Does churn vary across age groups and gender?
3. Which locations have higher customer churn?
4. How does customer lifetime relate to churn?
5. Does account balance influence customer churn?
6. Is credit card ownership associated with churn?
7. Are inactive customers more likely to leave than active customers?
8. Which customer segments should receive greater retention attention?

---

## Dataset Overview

The dataset contains **10,000 customer records** and includes information about customer demographics, account characteristics, financial information, and churn status.

### Key Variables

| Variable          | Description                                        |
| ----------------- | -------------------------------------------------- |
| CustomerId        | Unique customer identifier                         |
| Surname           | Customer surname                                   |
| Location          | Customer location                                  |
| Gender            | Customer gender                                    |
| Age               | Customer age                                       |
| Age Groups        | Categorized age groups                             |
| Tenure            | Number of years with the bank                      |
| Customer LifeTime | New, Mid-Term, or Long-Term customer               |
| Balance           | Customer account balance                           |
| Balance Groups    | Low, Medium, or High Balance                       |
| NumOfProducts     | Number of bank products owned                      |
| HasCrCard         | Indicates whether the customer has a credit card   |
| IsActiveMember    | Indicates whether the customer is an active member |
| EstimatedSalary   | Estimated customer salary                          |
| Exited            | Indicates whether the customer churned             |

The target variable is **Exited**, where `1` represents a churned customer and `0` represents a customer who remained with the bank.

---

## Data Cleaning Process

The dataset was prepared in Microsoft Excel before analysis.

### Cleaning and Preparation Steps

* Reviewed the raw dataset and its column structure.
* Removed unnecessary header formatting and prepared the data into a structured table.
* Checked for missing values.
* Checked for duplicate records.
* Reviewed data types and ensured numerical fields were suitable for analysis.
* Reviewed categorical variables for consistency.
* Created an **Age Groups** field to segment customers.
* Created **Customer LifeTime** categories based on tenure.
* Created **Balance Groups** to classify customers according to their account balance.
* Verified the cleaned dataset before creating PivotTables and charts.

The final cleaned dataset contained **10,000 records with no blank values or duplicate rows**.

<img width="401" height="255" alt="image" src="https://github.com/user-attachments/assets/87fa9160-93ad-4c1e-9946-08bbea8df152" />   <img width="365" height="255" alt="image" src="https://github.com/user-attachments/assets/0efb707c-37a9-472f-89ab-73619629ceb1" />

---

## Chart Analysis and Business Questions

### 1. Overall Churn Distribution

The overall churn rate was **20.37%**, meaning approximately one in five customers in the dataset had exited the bank, while **79.63% remained**. Customer churn represents a significant portion of the customer base and indicates a need to understand the characteristics of customers who leave.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/1d95b1bf-a544-4ed4-a220-9dc9b23fd8a8" />

---

### 2. Churn Rate by Age Group

The analysis showed differences in churn across age groups:

* **Seniors:** approximately 23.18%
* **Young Adults:** approximately 20.39%
* **Middle-Aged:** approximately 20.10%

Seniors recorded the highest churn rate, although they represent a much smaller portion of the dataset than the other age groups. Age appears to be associated with differences in churn, but the small number of senior customers should be considered when interpreting this result.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/7d42ad85-9252-4d62-bfcd-117202386cb5" />

---

### 3. Churn Rate by Gender

Female customers had a churn rate of approximately **25.07%**, compared with approximately **16.46% for male customers**. Female customers in this dataset experienced a higher churn rate than male customers. This difference could be investigated further alongside other factors such as age, location, balance, tenure, and product usage rather than treating gender alone as the cause of churn.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/01907a36-16d1-480c-967e-4015081751de" />

---

### 4. Churn Rate by Location

Churn varied across the five locations:

* **Port Harcourt:** approximately 22.00%
* **Lagos:** approximately 21.35%
* **Abuja:** approximately 19.92%
* **Enugu:** approximately 19.75%
* **Ibadan:** approximately 18.87%

Port Harcourt and Lagos recorded higher churn rates than the other locations, while Ibadan recorded the lowest. Location-specific customer experience, service accessibility, and engagement could be investigated to understand these differences.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/8999b990-695a-4e04-bf55-6a4caadd2d57" />

---

### 5. Churn Rate by Customer Lifetime

Customer lifetime was divided into New, Mid-Term, and Long-Term customers.

* **New customers:** approximately 21.15%
* **Mid-Term customers:** approximately 20.76%
* **Long-Term customers:** approximately 19.67%

New customers had the highest churn rate, while long-term customers had the lowest. Early-stage customers may require stronger onboarding, engagement, and relationship-building strategies.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/18981b33-b423-41b6-973e-2aa6d75d6220" />

---

### 6. Churn Rate by Balance Group

Churn differed considerably across balance groups:

* **High Balance:** approximately 25.96%
* **Medium Balance:** approximately 24.23%
* **Low Balance:** approximately 15.12%

High-balance customers recorded the highest churn rate, while low-balance customers had the lowest. High-value customers who show signs of disengagement may require closer monitoring because their departure could have a greater financial impact on the bank.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/95a96e08-40bc-413b-bbd1-c46850b93dc0" />

---

### 7. Churn Rate by Credit Card Ownership

Customers without a credit card had a churn rate of approximately **20.81%**, while customers with a credit card had a churn rate of approximately **20.18%**. The difference is relatively small, suggesting that credit card ownership alone does not show a strong difference in churn within this dataset.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/5c0dc8f1-2eeb-4228-96fc-46b6144de6d7" />

---

### 8. Churn Rate by Active Membership

Customer activity showed a more noticeable difference.

* **Inactive members:** approximately 26.85% churn
* **Active members:** approximately 14.27% churn

Inactive customers had a substantially higher churn rate than active customers. Customer engagement appears to be an important factor to investigate when developing retention strategies.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/1fa443fd-07ba-4a4d-8391-8a8bb5099c2e" />

---

## Dashboard Summary

The dashboard provides a consolidated view of GT Bank's customer churn situation.

### Key Dashboard KPIs

* **Total Customers:** 10,000 
* **Total Churn Rate:** 20.37%
* **Active Members:** 5,151
* **Customers Retained:** 79.63%
* **Customers Churned:** 20.37%

<img width="1500" height="650" alt="image" src="https://github.com/user-attachments/assets/2567eafe-6370-4a93-b85a-e0aaefee49f8" />

---

## Key Insights

1. **Overall churn:** 20.37% of customers in the dataset have exited the bank.

2. **Customer activity:** Inactive members recorded a much higher churn rate than active members, indicating a strong relationship between engagement and retention.

3. **Balance:** High-balance customers had a higher churn rate than low-balance customers, making high-value customer retention an important consideration.

4. **Gender:** Female customers recorded a higher churn rate than male customers in the dataset.

5. **Location:** Port Harcourt and Lagos recorded the highest churn rates among the five locations analyzed.

6. **Customer lifetime:** New customers showed a higher churn rate than long-term customers, suggesting that early customer engagement may be important.

7. **Credit cards:** Churn rates were relatively similar between customers with and without credit cards.

---

## Recommendations

### 1. Strengthen Customer Engagement

Develop targeted engagement campaigns for inactive customers through personalized communication, relevant offers, and regular relationship management.

### 2. Protect High-Value Customers

Monitor high-balance customers for signs of disengagement and provide personalized retention offers or relationship-management support where appropriate.

### 3. Improve New Customer Onboarding

Introduce stronger onboarding and early-stage engagement programs to help new customers understand and use available banking services.

### 4. Investigate Location-Based Churn

Conduct further analysis of customer experience, service accessibility, and product usage in higher-churn locations such as Port Harcourt and Lagos.

### 5. Develop Customer Segmentation

Combine factors such as age, balance, tenure, activity, and product ownership to identify customer segments requiring different retention approaches.

### 6. Monitor Customer Activity

Use customer activity indicators to identify customers becoming less engaged and intervene before they become likely to churn.

### 7. Investigate High-Churn Segments Further

The analysis identifies relationships between customer characteristics and churn, but these relationships do not by themselves establish causation. Further analysis could examine combinations of variables to better understand why customers leave.

---

## Conclusion

The GT Bank Customer Churn Analysis provides a data-driven view of customer attrition across different demographic, financial, geographic, and engagement characteristics.

The analysis found an overall churn rate of **20.37%**, with notable differences across customer activity, balance groups, gender, location, age, and customer lifetime. In particular, inactive customers and high-balance customers showed higher churn rates than their respective comparison groups.

The dashboard transforms these findings into an easy-to-understand visual report that can help stakeholders identify areas requiring further investigation and develop more targeted customer retention strategies.

Overall, the project demonstrates how **Excel, data cleaning, PivotTables, data visualization, and dashboard development** can be used to transform raw customer data into meaningful business insights.

---

