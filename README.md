# Customer Churn Analysis Dashboard | FutureInterns Task 2

## Project Overview

This project explores customer churn for a subscription-based telecom company. I used the data to identify the customer groups most likely to leave, understand what may be driving churn, and turn those findings into practical retention ideas.

This project is part of Task 2 of the FutureInterns Data Science & Analytics internship.

## Repository Structure

```text
data/
dashboard/
images/
reports/
README.md
```

## Business Problem

Customer churn happens when customers stop using a company's service. For a subscription business, even a small increase in churn can affect revenue, growth, and long-term customer value.

This analysis focuses on a few key questions:

- What is the overall customer churn rate?
- Which customer segments have the highest churn?
- How does contract type affect churn?
- How does customer lifetime, or tenure, affect churn?
- Which services or payment methods are linked to higher churn?
- What actions can reduce customer loss?

## Dataset

Dataset used: **Telco Customer Churn Dataset**

The dataset includes customer details such as:

- Customer ID
- Gender
- Senior citizen status
- Partner and dependent status
- Tenure
- Phone and internet services
- Contract type
- Payment method
- Monthly charges
- Total charges
- Churn status

## Tools Used

- Microsoft Excel
- Power BI
- GitHub

## Data Cleaning

I prepared the data in Excel before building the analysis. The main cleaning steps were:

- Split the original comma-separated data into separate columns.
- Checked for blank values.
- Formatted numeric and currency columns.
- Applied filters to all header columns.
- Adjusted column widths and row heights for readability.
- Created a `Churn Flag` helper column:
  - `1` for customers who churned
  - `0` for customers who stayed
- Created a `Tenure Group` column to group customers by how long they had stayed with the company.

## Key Metrics

| Metric | Value |
|---|---:|
| Total Customers | 7,043 |
| Churned Customers | 1,869 |
| Retained Customers | 5,174 |
| Overall Churn Rate | 27% |

## Key Insights

### 1. Overall Churn

The overall churn rate is **27%**, which means roughly one in every four customers left the company.

### 2. Contract Type

Contract length makes a clear difference. Month-to-month customers have the highest churn rate at **43%**, while one-year contracts drop to **11%** and two-year contracts fall even further to **3%**.

This suggests that longer contracts are strongly linked to better retention.

### 3. Tenure Group

Customers in their first 12 months have the highest churn rate at **47%**. After that, churn steadily decreases as tenure increases.

In short, the first year is the riskiest period in the customer journey.

### 4. Payment Method

Customers using electronic check have the highest churn rate at **45%**. Customers using credit card, bank transfer, or mailed check show noticeably lower churn.

### 5. Internet Service

Fiber optic customers churn at **42%**, much higher than DSL customers at **19%** and customers with no internet service at **7%**.

### 6. Tech Support

Customers without tech support churn at **42%**, compared with only **15%** for customers who have tech support.

## Business Recommendations

- Encourage month-to-month customers to move into annual or two-year contracts through discounts, loyalty offers, or bundled benefits.
- Prioritize retention campaigns for customers in their first 12 months.
- Investigate why electronic check users churn more often, then promote more stable payment options.
- Review fiber optic pricing, service quality, and customer expectations.
- Position tech support as a retention feature, especially for high-risk customers.
- Build onboarding and follow-up programs for early-stage customers.

## Dashboard Preview

The Power BI dashboard has been added to this repository:

- Dashboard file: [dashboard/Telco Churn Analysis Dashboard.pbix](dashboard/Telco%20Churn%20Analysis%20Dashboard.pbix)
- Dashboard screenshot: [images/Telco Customer Churn Analysis.png](images/Telco%20Customer%20Churn%20Analysis.png)

![Telco Customer Churn Analysis Dashboard](images/Telco%20Customer%20Churn%20Analysis.png)
