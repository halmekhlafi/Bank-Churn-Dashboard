## Problem statement 
The bank is experiencing customer attrition and seeks to understand the underlying behaviors and patterns driving churn. By analyzing customer subscriptions, service usage, and demographic details, the goal is to gain insights into how customers experience the bank's services and what factors contribute to their decision to leave

## Data Preparation & Business Dashboard Insights
🧼 Data Cleaning & Transformation
After importing and merging raw Excel data, the following preprocessing steps were applied to ensure consistency and readiness for visualization:

### ✅ Standardizing Data
Geography Cleanup: Unified inconsistent values ('FRA', 'French') into 'France'.

Duplicate Columns: Merged identical tenure columns into a single Tenure field.

### 💶 Formatting & Type Conversion
Removed the Euro symbols (€) and converted EstimatedSalary and Balance columns to numeric types for accurate calculation.

### 🧓 Age Handling
Replaced missing/infinite values in Age with 0 and converted to int.

Binned Age into 5 age groups for segmentation (e.g., 18–31, 32–46, etc.).

### 💾 Export Ready
The final dataset was prepared for visualization and optionally saved as a CSV.

# df.to_csv('Bank_Churn_Messy.csv', index=False)
#### 📈 Business Dashboard Insights

This Power BI dashboard provides a comprehensive view of customer churn behavior, helping decision-makers identify key areas of focus. Below are the core business insights extracted from the visuals:

## 🧠 Key Metrics
Total Customers: 9,999

Total Churned: 2,038 customers (~20%)

Female Churn Rate: 56%

Male Churn Rate: 44%

## 📌 Notable Findings
1. Churn by Gender:

A higher proportion of female customers are leaving compared to males.

Suggests the need to review services or communications targeting female segments.

2. Churn by Age Group:

Ages 32–46 and 18–31 represent the largest churn segments.

Younger age groups may need better onboarding or engagement strategies.

3. Churn by Geography:

Germany and France have the highest churn numbers (~814 each), whereas Spain shows significantly lower churn (~413).

Indicates potential issues with regional service satisfaction or market competition.

4. Tenure vs Churn Rate:

Customers with shorter tenures (0–3 years) are more likely to churn.

Highlights the importance of strengthening early customer relationships.

5. Estimated Salary & Balance:

Higher salaries and balances do not significantly correlate with reduced churn.

Suggests churn is driven more by experience or service than by financial status.

6. Customer Activity:

Customers without a credit card and those who are inactive churn more frequently.

Encouraging product engagement and credit usage may improve retention.

### 💡 Business Value
This dashboard empowers business teams to:

-Target at-risk demographics with tailored retention campaigns.

-Improve onboarding experiences for new customers.

-Localize service improvements based on geography-specific churn patterns.

-Customize accounts based on the customer's financial 

-Align product and credit offerings with engagement and loyalty goals.

