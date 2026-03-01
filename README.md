**Customer Behavior, Revenue and Churn Analysis**
_____________________________________________________________________________________________________________________________________________________________________

**Executive Summary**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

This project delivers an end-to-end customer behaviour intelligence solution for an e-commerce business. Using Python for structured data cleaning and feature engineering, and Power BI for interactive dashboard development, the project transforms raw customer data into actionable business insights. The solution enables stakeholders to monitor revenue distribution, engagement patterns, and behavioural risk indicators in real time.

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

**Project Architecture**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
Raw Dataset

     ↓
     
Python (Data Cleaning & Feature Engineering)

     ↓
     
Cleaned Dataset (CSV)

     ↓
     
Power BI (Data Model + DAX Measures)

     ↓
Interactive Business Dashboard

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
- Calculation of Different KPIs ()
- Behavioural indicators supporting segmentation analysis

The cleaned dataset was exported and used as the reporting layer input.

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
