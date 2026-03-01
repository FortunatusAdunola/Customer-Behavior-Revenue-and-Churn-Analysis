<h1>Customer Behavior, Revenue and Churn Analysis</h1>

**Executive Summary**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

This project delivers a multi-page Business Intelligence solution designed to help an e-commerce company monitor revenue performance, customer engagement, churn risk, and cart abandonment behaviour. Using Python for structured data preparation and Power BI for dashboard development, the solution transforms raw behavioural data into executive-level KPIs and interactive reporting pages for data-driven decision-making.

**Business Problem**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

E-commerce businesses face three core challenges:

- Revenue concentration among few customers
- Declining engagement over time
- Lack of visibility into behavioural risk segments

This project aims to:

- Segment customers based on revenue contribution
- Identify engagement patterns influencing performance
- Deliver a dynamic dashboard for decision-makers

**BI Architecture**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
```
Raw Dataset
      ↓
Python (Data Cleaning & Feature Engineering)
      ↓
Clean Analytical Dataset (CSV Export)
      ↓
Power BI (Data Model + DAX Measures)
      ↓
Interactive Multi-Page Dashboard
``` 

**Data Preparation (Python)**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

All preprocessing was completed in Python before importing into Power BI to ensure:

- Reproducibility
- Data integrity
- Clean analytical foundation

**Key Data Preparation Activities:**

- Missing value assessment and treatment
- Data type validation
- Duplicate checks
- Outlier review
- Revenue segmentation using quantile logic
- Engagement classification using behavioural thresholds

Engineered features include:

- Revenue Segment (Low / Mid / High Value)
- Engagement Level
- Calculation of Different KPIs 
- Behavioural indicators supporting segmentation analysis

The cleaned dataset was exported and used as the reporting layer input.

**Power BI Dashboard Overview**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
The dashboard is structured into four business-focused reporting pages.


<h3>Page 1: Customer Behavior & Revenue Analysis</h3>

_Purpose: Identify behavioural drivers of revenue._

**Executive KPIs**

- Total Customers: 50K
- Purchase Rate: 13.11
- Churn Rate: 28.90%
- Total Revenue: $80.92M
- Average Order Value: $123.12
- Cart Abandonment: 57.08%
- Average CLV: $1.44K

**Key Visuals**

- Purchases by Customer Segment
- Session Duration vs Login Frequency
- Total Purchases vs Pages Per Session
- Payment Method vs Lifetime Value

**Business Value**

Helps management understand how engagement behaviour influences revenue contribution.

<img width="1162" height="638" alt="image" src="https://github.com/user-attachments/assets/93fb2adf-db25-44c5-8337-754942d3bb56" />


<h3>Page 2: Revenue & Purchase Behaviour</h3>

_Purpose: Analyse revenue generation patterns._

**Key Visuals**

- Total Revenue by Customer Segment
- Revenue by Gender
- Lifetime Value by Membership Years
- Revenue vs Discount Usage

**Insights Enabled**

- Revenue concentration risk analysis
- Long-term value trend identification
- Discount effectiveness evaluation

<img width="1170" height="647" alt="image" src="https://github.com/user-attachments/assets/dd5a1ff5-fe4c-43fb-92f6-c12bc14afc34" />



<h3>Page 3: Churn & Retention Analysis</h3>

_Purpose: Identify risk indicators and quantify revenue loss._

**Key Visuals**

- Churned vs Active Customers
- Churn by Login Frequency
- Churn Rate by Customer Segment
- Revenue Lost from Churned Customers
- Engagement Level vs Churn

**Business Value**

- Enables retention strategy design
- Quantifies financial impact of churn
- Highlights early behavioural risk signals

<img width="1166" height="641" alt="image" src="https://github.com/user-attachments/assets/380f5ece-7112-4b8c-ad8d-ea028d095674" />


<h3>Page 4: Cart Abandonment & Conversion Analysis</h3>

_Purpose: Improve checkout conversion performance._

**Key Visuals**

- Churned vs Cart Abandonment Level
- Cart Abandonment Rate vs Pages Per Session
- Purchases by Customer Segment
- Customer Distribution by Abandonment Level

**Business Value**

- Identifies behavioural drivers of abandonment
- Supports UX optimisation decisions
- Improves funnel conversion strategy

<img width="1165" height="645" alt="image" src="https://github.com/user-attachments/assets/68ac70ba-d550-4343-96c6-87c2baf0641a" />


**Power BI Data Modelling**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

The cleaned dataset was imported into Power BI where additional modelling was performed.

**Data Model Design**

- Optimised for reporting efficiency
- Clear separation between raw columns and calculated measures

**DAX Measures & Calculations**

Custom DAX measures were created to enhance business intelligence capability:
- Abandonment Level (Column)
- Active Customers
- Average Cart Abandonment Rate
- Churn Rate
- Churn Status (Column)
- Churned Customers
- Purchase Frequency
- Total Customers
- Total Revenue

Calculated columns were created for dynamic segmentation and filtering. These measures also allow dynamic slicing by customer behaviour and revenue category.

**Key Business Insights**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

1. Revenue is highly concentrated among high-value customers.
2. Engagement metrics strongly correlate with purchase behaviour.
3. Churn rate of 28.9% represents significant revenue risk.
4. Cart abandonment rate (57%) indicates conversion optimisation opportunity.
5. Login frequency is a strong behavioural predictor of churn.

**Strategic Recommendations**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

1. Protect high-value customers through loyalty initiatives.
2. Deploy retention campaigns targeting mid-value segment.
3. Monitor engagement decline as an early churn signal.
4. Optimise checkout funnel to reduce abandonment.
5. Reassess discount strategy based on behavioural impact.

**Tools & Technologies**
-----------------------------------------------------------------------------------------------------------------------------------------------------------------

- Python (Pandas, NumPy)
- Jupyter Notebook
- Power BI
- DAX

**How to Use**
-----------------------------------------------------------------------------------------------------------------------------------------------------------------

- Review Python notebook for data preparation logic
- Open Power BI file (.pbix) for interactive exploration
- Use slicers to analyse segment-specific performance
