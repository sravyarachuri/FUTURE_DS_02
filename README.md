# 📊 Customer Retention & Churn Analysis

### Future Interns – Data Science & Analytics Internship (Task 2)

---

## Project Overview

This project was completed as part of the **Future Interns Data Science & Analytics Internship – Task 2: Customer Retention & Churn Analysis**.

The objective was to analyze telecommunications customer data to understand churn patterns, customer retention, subscription behavior, and factors associated with customers leaving the service.

The project uses **Microsoft Power BI** to build an interactive dashboard that presents customer churn KPIs and explores customer behavior across contract types, internet services, payment methods, tenure, monthly charges, and demographic segments.

---

## Business Problem

Customer churn is a major challenge for subscription-based businesses. Losing customers can affect recurring revenue, increase customer acquisition costs, and reduce long-term business growth.

This project addresses the following key business questions:

- What percentage of customers have churned?
- How many customers have been retained?
- Which contract type has the highest churn rate?
- How do internet service and payment methods relate to customer churn?
- How does customer tenure differ between churned and retained customers?
- Are monthly charges associated with customer churn?
- Which customer segments may require targeted retention strategies?

---

## Dataset

**Dataset:** Telco Customer Churn

The dataset contains customer demographic information, subscribed telecommunications services, contract details, payment methods, tenure, monthly charges, total charges, and churn status.

**Source:**&#x20;- https://www.kaggle.com/datasets/blastchar/telco-customer-churn

### Key Attributes

| Column          | Description                                                        |
| --------------- | ------------------------------------------------------------------ |
| customerID      | Unique identifier for each customer                                |
| gender          | Customer gender                                                    |
| SeniorCitizen   | Indicates whether the customer is a senior citizen                 |
| Contract        | Customer's subscription contract type                              |
| InternetService | Internet service category: DSL, Fiber optic, or No                 |
| PaymentMethod   | Method used to pay for the service                                 |
| tenure          | Length of time the customer has stayed with the company, in months |
| MonthlyCharges  | Recurring monthly amount charged to the customer                   |
| TotalCharges    | Total charges recorded for the customer                            |
| Churn           | Indicates whether the customer left the service (Yes/No)           |

---

## Data Preparation

The project uses a cleaned customer dataset in Power BI for analysis.

### Processing and Analysis

- Used the cleaned customer dataset in Power BI.
- Created KPI measures for total customers, retained customers, churned customers, churn rate, and retention rate.
- Analyzed customer churn across contract types and demographic segments.
- Compared churn counts across internet service and payment methods.
- Examined average customer tenure and monthly charges by churn status.
- Added interactive slicers to explore customer segments.

---

## Dashboard KPIs

The following values are from the overall, unfiltered Power BI dashboard.

| KPI                         |  Value |
| --------------------------- | -----: |
| Total Customers             |  7,032 |
| Active / Retained Customers |  5,163 |
| Churned Customers           |  1,869 |
| Overall Churn Rate          | 26.58% |
| Overall Retention Rate      | 73.42% |

---

## Dashboard Features

### Interactive Filters

- Gender
- Contract Type
- Internet Service
- Senior Citizen Status

### Visualizations

- Customer Churn Distribution
- Contract Type vs Customer Churn
- Internet Service vs Customer Churn
- Payment Method vs Customer Churn
- Customer Tenure Distribution
- Average Monthly Charges by Churn

---

## Dashboard Preview
<img width="935" height="823" alt="dashboard_image" src="https://github.com/user-attachments/assets/06652081-f14e-4823-8ae9-6b6ee91764bc" />



---

## Key Business Insights

### Overall Customer Churn

- The dataset contains **7,032 customers**.
- A total of **1,869 customers churned**, representing a churn rate of **26.58%**.
- The remaining **5,163 customers were retained**, resulting in a retention rate of **73.42%**.

### Contract Type Analysis

Contract type shows a substantial difference in observed churn rates.

| Contract Type  | Total Customers | Churned Customers | Churn Rate |
| -------------- | --------------: | ----------------: | ---------: |
| Month-to-month |           3,875 |             1,655 |     42.71% |
| One year       |           1,472 |               166 |     11.28% |
| Two year       |           1,685 |                48 |      2.85% |

**Key finding:** Month-to-month customers have the highest churn rate at **42.71%**, while two-year contract customers have the lowest at **2.85%**.

This suggests that customers on shorter-term contracts may need additional retention attention. The observed relationship does not prove that contract length alone causes churn.

### Internet Service Analysis

- The dashboard compares churned and retained customer counts for Fiber optic, DSL, and customers without internet service.
- Fiber optic has the largest visible churn count in the overall dashboard.
- Customer counts alone do not establish which internet service has the highest churn rate. Category-specific churn rates would be needed for a fair risk comparison.

### Payment Method Analysis

- Electronic check has the largest visible churn count among the payment methods in the overall dashboard.
- The other payment categories include mailed check, bank transfer, and credit card.
- Churn counts should not be interpreted as churn rates without comparing churned customers against the total customers in each payment category.

### Customer Tenure Analysis

- In the overall dashboard view, churned customers have an average tenure of approximately **18 months**.
- Customers who did not churn have an average tenure of approximately **38 months**.

**Key finding:** Churned customers have a shorter average relationship with the company in the overall dataset, highlighting the importance of understanding customer experience during the early stages of the relationship.

### Monthly Charges Analysis

- Customers who churned had average monthly charges of approximately **74**.
- Customers who stayed had average monthly charges of approximately **61**.

**Key finding:** Churned customers had higher average monthly charges in the overall dashboard. Pricing and perceived value may warrant further investigation, but the chart does not prove that higher charges caused churn.

### Gender Analysis

| Gender | Total Customers | Churned Customers | Churn Rate |
| ------ | --------------: | ----------------: | ---------: |
| Female |           3,483 |               939 |     26.96% |
| Male   |           3,549 |               930 |     26.20% |

**Key finding:** Churn rates are similar for female and male customers, with a difference of approximately 0.76 percentage points.

### Senior Citizen Analysis

| Segment            | Total Customers | Churned Customers | Churn Rate |
| ------------------ | --------------: | ----------------: | ---------: |
| Senior citizen     |           1,142 |               476 |     41.68% |
| Non-senior citizen |           5,890 |             1,393 |     23.65% |

**Key finding:** The senior-citizen segment has a higher observed churn rate than the non-senior segment. Further analysis is needed to understand the possible reasons.

---

## Business Recommendations

### Prioritize Month-to-Month Customers

Offer suitable renewal incentives, loyalty benefits, and longer-term plan options to month-to-month customers who may benefit from them.

### Strengthen Early Customer Retention

Improve onboarding, customer support, and early engagement. Monitor churn across tenure groups to identify when customers are most likely to leave.

### Investigate Senior-Citizen Churn

Examine service experience, contract types, pricing, and support needs within this segment before developing targeted retention initiatives.

### Review Pricing and Perceived Value

Assess whether customers with higher monthly charges feel they receive sufficient value from their subscriptions. Consider suitable plan reviews and transparent billing communication.

### Investigate Internet Service and Payment Segments

Calculate churn rates within each internet-service and payment-method category before deciding which groups have the highest churn risk.

### Monitor Retention KPIs

Track churn rate, retention rate, and contract-level churn regularly to evaluate the effectiveness of retention initiatives.

---

## Technology Stack

- Microsoft Power BI
- Power Query, if used for data preparation
- DAX for KPI calculations
- Microsoft Excel for dataset storage and preparation
- Jupyter Notebook, if used in the final analysis
- GitHub for project documentation and version control

---

## Repository Structure

```text
FUTURE_DS_02/
│
├── Dashboard/
│   └── Customer_Churn_Analysis.pbix
│
├── Dataset/
│   └── Cleaned_Telco_Customer_Churn.xlsx
│
├── Images/
│   └── dashboard_image.png
│
├── Notebooks/
│   └── Customer_Churn_Analysis.ipynb
│
├── Reports/
│   └── Customer_Retention_Churn_Analysis_Report_Task2.pdf
│
└── README.md
```

---

## Deliverables

- Interactive Power BI Customer Retention & Churn Analysis Dashboard
- Customer churn KPI analysis
- Segment-level churn findings
- Business recommendations for customer retention
- Project report
- GitHub project documentation

---

## Project Outcome

This project transformed telecommunications customer data into an interactive business intelligence dashboard for understanding customer churn and retention.

The analysis identified a **26.58% overall churn rate** and highlighted substantial differences in churn across contract types. Month-to-month customers showed the highest observed churn rate, while two-year contract customers showed the lowest.

The dashboard also revealed differences in average tenure, monthly charges, and churn across demographic segments. These findings provide a starting point for further investigation and evidence-based retention planning.

The final solution supports exploratory analysis and can help business stakeholders identify customer segments that may benefit from targeted retention initiatives.

---

## Author

**Sravya Rachuri**

Future Interns – Data Science & Analytics Internship

**Task 2: Customer Retention & Churn Analysis**
