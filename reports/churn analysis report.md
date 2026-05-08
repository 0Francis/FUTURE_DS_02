# Customer Churn Analysis Report

## 1. Objective

This report looks at customer churn patterns for a subscription-based telecom business. The main goal is to understand which customers are most likely to leave, what factors are connected to churn, and where the business can focus its retention efforts.

The analysis also looks at customer lifetime trends so the business can see how churn changes as customers stay longer.

## 2. Dataset Summary

The dataset contains **7,043 customer records**. Each row represents one customer and includes demographic details, subscription information, services used, payment method, charges, tenure, and churn status.

The main target column is `Churn`, where:

- `Yes` means the customer left.
- `No` means the customer stayed.

## 3. Data Preparation

The dataset was cleaned and prepared in Excel.

The preparation steps included:

- Splitting comma-separated values into 21 columns.
- Formatting numeric and currency columns.
- Checking for blank values.
- Applying filters to all columns.
- Creating a `Churn Flag` column for churn rate calculations.
- Creating a `Tenure Group` column to analyze customer lifetime patterns.
- Building an interactive Power BI dashboard to summarize churn KPIs and segment-level patterns.

## 4. Overall Churn Performance

The dataset contains:

| Customer Status | Count |
|---|---:|
| Retained Customers | 5,174 |
| Churned Customers | 1,869 |
| Total Customers | 7,043 |

The overall churn rate is **27%**.

This means approximately one in every four customers has left the business, which is a meaningful retention challenge for a subscription-based company.

## 5. Churn by Contract Type

| Contract Type | Customers | Churn Rate |
|---|---:|---:|
| Month-to-month | 3,875 | 43% |
| One year | 1,473 | 11% |
| Two year | 1,695 | 3% |

Month-to-month customers have the highest churn rate by a wide margin. Customers on longer contracts are much less likely to churn.

### Insight

Contract type appears to be one of the strongest churn indicators. The longer contracts are closely linked with stronger customer retention.

## 6. Churn by Tenure Group

| Tenure Group | Customers | Churn Rate |
|---|---:|---:|
| 0-12 months | 2,186 | 47% |
| 13-24 months | 1,024 | 29% |
| 25-48 months | 1,594 | 20% |
| 49+ months | 2,239 | 10% |

Customers in their first 12 months have the highest churn rate. Churn then decreases steadily as customer tenure increases.

### Insight

New customers are the most vulnerable group. The first year should be treated as a critical retention window, with more onboarding, support, and follow-up.

## 7. Churn by Payment Method

| Payment Method | Customers | Churn Rate |
|---|---:|---:|
| Electronic check | 2,365 | 45% |
| Mailed check | 1,612 | 19% |
| Bank transfer automatic | 1,544 | 17% |
| Credit card automatic | 1,522 | 15% |

Electronic check users have the highest churn rate, while customers using automatic payment methods show lower churn.

### Insight

Payment method may be linked to customer stability. Automatic payments could reduce friction and may also reflect customers who are more committed to staying.

## 8. Churn by Internet Service

| Internet Service | Customers | Churn Rate |
|---|---:|---:|
| Fiber optic | 3,096 | 42% |
| DSL | 2,421 | 19% |
| No internet service | 1,526 | 7% |

Fiber optic customers show the highest churn rate among the internet service groups.

### Insight

The business should investigate whether fiber optic customers are facing mostly pricing concerns or service quality issues, or expectations that are not being met. 

## 9. Churn by Tech Support

| Tech Support | Customers | Churn Rate |
|---|---:|---:|
| No | 3,473 | 42% |
| Yes | 2,044 | 15% |
| No internet service | 1,526 | 7% |

Customers without tech support churn at a much higher rate than customers who have tech support.

### Insight

Tech support appears to play an important role in retention. Customers who receive support may feel more confident staying with the service.

## 10. Key Findings

- The overall churn rate is 27%.
- Average customer tenure is 32 months.
- Month-to-month customers have the highest churn rate at 43%.
- Customers in their first 12 months have the highest churn rate at 47%.
- Electronic check users have the highest churn rate at 45%.
- Fiber optic customers have a high churn rate of 42%.
- Customers without tech support have a high churn rate of 42%.
- Longer tenure and longer contracts are linked to stronger retention.

## 11. Recommendations

### 1. Convert Month-to-Month Customers

The business should encourage month-to-month customers to move to one-year or two-year contracts using loyalty discounts, upgrade benefits, or bundled offers. Since this group has the highest churn rate, even a small improvement here could have a strong impact.

### 2. Improve First-Year Retention

Customers in their first 12 months are most likely to churn. The company should strengthen onboarding through welcome messages, check-ins, early support, and targeted offers before customers disengage.

### 3. Promote Automatic Payment Methods

Electronic check users have the highest churn rate. The company should encourage customers to use automatic bank transfer or credit card payments, possibly through small incentives or easier setup.

### 4. Investigate Fiber Optic Churn

Fiber optic customers churn at a high rate. The business should review service quality, pricing, customer complaints, and competitor offers to understand what is pushing these customers away.

### 5. Position Tech Support as a Retention Tool

Customers with tech support churn less. The company should promote tech support bundles to high-risk customers, especially newer customers and those on month-to-month contracts.

## 12. Power BI Dashboard

An interactive Power BI dashboard was created to make the churn analysis easier to explore and present.

The dashboard includes:

- KPI cards for total customers, churned customers, churn rate, and average tenure.
- Churn rate by contract type.
- Churn rate by tenure group.
- Churn rate by payment method.
- Churn rate by internet service.
- Churn rate by tech support.
- Slicers for contract type, tenure group, and internet service.

Dashboard file: [../dashboard/Telco Churn Analysis Dashboard.pbix](../dashboard/Telco%20Churn%20Analysis%20Dashboard.pbix)

Dashboard screenshot: [../images/Telco Customer Churn Analysis.png](../images/Telco%20Customer%20Churn%20Analysis.png)

![Telco Customer Churn Analysis Dashboard](../images/Telco%20Customer%20Churn%20Analysis.png)

## 13. Conclusion

The analysis shows that churn is highest among early-stage customers, especially those on month-to-month contracts, using electronic check payments, lacking tech support, or using fiber optic internet service.

The Power BI dashboard supports these findings by bringing the main KPIs, churn segments, and interactive filters into one view.

To reduce churn, the business should focus on stronger early engagement, contract upgrades, better payment experiences, tech support promotion, and a closer review of the fiber optic customer experience.
