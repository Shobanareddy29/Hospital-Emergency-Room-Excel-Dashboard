# 🏥 Hospital Emergency Room Dashboard using Microsoft Excel

## 📌 Project Overview

The **Hospital Emergency Room Dashboard** is an interactive Excel dashboard developed to analyze Emergency Room (ER) operations and provide actionable insights for healthcare management.

The project demonstrates the complete data analytics workflow—from importing and cleaning data to building an interactive dashboard using **Power Query**, **Power Pivot**, **Pivot Tables**, **Pivot Charts**, and **DAX**.

The dashboard enables users to monitor patient volume, waiting time, admission status, patient satisfaction, demographics, and department referrals through dynamic visualizations and slicers.



# 🎯 Project Purpose

The objective of this project is to build an interactive Hospital Emergency Room dashboard that helps healthcare stakeholders monitor operational performance and improve decision-making.

The dashboard provides insights into:

- Total patients visiting the Emergency Room
- Average patient waiting time
- Patient satisfaction score
- Admitted vs Non-admitted analysis
- Gender distribution
- Age group distribution
- Department referrals
- Daily patient trends

# 🛠 Project Workflow

The dashboard was developed following the complete Business Intelligence workflow.

### 1️⃣ Business Requirement Gathering

- Understand the business problem
- Identify required KPIs
- Define dashboard requirements

### 2️⃣ Data Understanding

- Explore hospital emergency room dataset
- Understand data fields
- Identify missing values and inconsistencies

### 3️⃣ Data Connection

- Imported dataset using **Power Query**
- Connected Excel data source
- Prepared data for transformation

### 4️⃣ Data Cleaning & Data Quality Check

Performed data transformation using Power Query:

- Removed unnecessary columns
- Corrected data types
- Cleaned missing values
- Standardized data
- Validated dataset

### 5️⃣ Calendar Table Creation

Created a dynamic Calendar Table using Power Query for proper time-based analysis.

```Power Query
List.Dates(#date(2023,1,1),731,#duration(1,0,0,0))
```

### 6️⃣ Data Modeling

Created relationships between:

- Hospital Emergency Room Data
- Calendar Table

using **Power Pivot Data Model**.


### 7️⃣ DAX Calculations

Created calculated columns using DAX.

#### Age Group

```DAX
IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))
```

#### Patient Attend Status

```DAX
IF([Patient Waittime]<30,"Within Time","Delay")
```

### 8️⃣ Pivot Tables & Dashboard Layout

Developed:

- Pivot Tables
- Pivot Charts
- KPI Cards
- Interactive Slicers
- Dashboard Layout


### 9️⃣ Chart Development

Created visualizations including:

- Patient Admission Status
- Age Group Distribution
- Daily Patient Trend
- Gender Analysis
- Department Referral Analysis
- Patient Attend Status


### 🔟 Dashboard Development

Designed an interactive dashboard featuring:

- Dynamic KPI Cards
- Month Slicer
- Year Slicer
- Interactive Charts
- Professional Healthcare Theme

### 1️⃣1️⃣ Insights Generation

The dashboard enables users to quickly identify:

- Patient admission trends
- Peak patient days
- Average waiting time
- Patient satisfaction
- Department referral patterns
- Gender distribution
- Age group trends

# 📊 Key Performance Indicators (KPIs)

✔ Number of Patients

✔ Average Wait Time

✔ Patient Satisfaction Score

✔ Admission Status

✔ Patient Attend Status

✔ Gender Analysis

✔ Department Referral Analysis

✔ Age Group Distribution

✔ Daily Patient Trends


# 🛠 Tools & Technologies

- Microsoft Excel
- Power Query
- Power Pivot
- DAX
- Pivot Tables
- Pivot Charts
- Data Modeling
- Slicers
- Conditional Formatting

# 📈 Business Insights

Using this dashboard, stakeholders can:

- Monitor Emergency Room performance
- Improve patient experience
- Reduce patient waiting time
- Analyze patient demographics
- Track hospital admission trends
- Monitor department workload
- Support data-driven healthcare decisions

# 💡 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Data Modeling
- DAX Calculations
- Dashboard Development
- Data Visualization
- Healthcare Analytics
- Business Intelligence
- Excel Reporting

# 👩‍💻 Author

**Shobana Reddy**

**M.Sc. Data Science**

Skills:
- Microsoft Excel
- SQL
- Power BI
- Python
- Data Analytics

## Acknowledgements

This project was developed as part of my learning journey in Microsoft Excel, Power Query, and Power Pivot.

The overall dashboard concept and learning guidance were inspired by the excellent tutorial series by Satish Dhawale.
I extended the project by recreating the dashboard independently for practice and portfolio purposes.

⭐ If you found this project useful, please consider giving it a Star!
