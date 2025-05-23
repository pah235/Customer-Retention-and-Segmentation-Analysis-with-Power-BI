# 📊 Customer Retention & Segmentation Analysis with Power BI

**Project Overview**
This portfolio project showcases a comprehensive Customer Retention Analysis and Customer Segmentation Analysis using Power BI. It leverages a robust data warehouse to provide actionable insights for improving customer loyalty and optimizing marketing strategies.

![image](https://github.com/user-attachments/assets/96c09294-4273-4901-bdc4-e9d4b87a147f)

---
- 👉 **You can access the visualization PDFs of Power BI report** [**here**](https://github.com/pah235/Customer-Retention-and-Segmentation-Analysis-with-Power-BI/blob/main/Customer%20Retention%20and%20Segmentation%20Analysis%20Report.pdf)
- 👉 **You can access the interactive Power BI report** [**here**](https://drive.google.com/file/d/1Ov8AOFs5xY9Nd_fRp7a-kp1jJdEFBOTB/view?usp=sharing)

## 🧰 A. Key Project Information

### 1. Tools & Skills Used
- Power Query: Applied extensive knowledge of Power Query for efficient data transformation, cleaning, and preparation.
- Data Modeling: Utilized advanced data modeling techniques to create a suitable and optimized data model for analysis.
- DAX (Data Analysis Expressions): Developed complex DAX measures and calculated columns to derive key performance indicators (KPIs) and metrics.
- Data Visualization: Designed and implemented appropriate chart types and visuals to effectively present analytical insights.
- Report Interactivity: Incorporated essential report functionalities such as Drill-down, Tooltips Page, Drill-through, Buttons, Bookmarks, and Parameter utilization to enhance user experience.
- Report Design: Created a complete and polished report layout suitable for presentation and stakeholder communication.

### 2. Project Introduction
This project is built upon a comprehensive Data Warehouse that captures the entire business process, from raw material procurement and manufacturing to sales.

#### a) About the Company: Contoso Corporation
Contoso Corporation is a multinational enterprise headquartered in Paris. It operates as a manufacturing, sales, and support organization, offering over 100,000 products. Contoso sells through two primary channels:
- Store (Physical Retail): Direct sales at brick-and-mortar retail locations.
- Online (E-commerce): Sales via website or e-commerce platforms.
Contoso primarily operates in the consumer electronics and accessories retail sector, including: Laptops, Desktops, Game Consoles, Mobile Phones, Accessories, Software, TVs & Media Devices.

#### b) Company Data Description: ContosoRetailDW
ContosoRetailDW (Contoso Retail Data Warehouse) is the centralized data warehouse for Contoso Corporation, provided by Microsoft, contains historical data on sales, inventory, promotions, and customers.
- **Source:** [Microsoft](https://www.microsoft.com/en-us/download/details.aspx?id=18279)
= **Key Components of ContosoRetailDW:**
#### 🔹 Fact Tables
| Table | Description |
|-------|-------------|
| `FactSales` | In-store sales transactions |
| `FactOnlineSales` | Online transaction data |
| `FactSalesQuota` | Sales targets by employee/time |
| `FactInventory` | Inventory levels |
| `FactExchangeRate` | Currency exchange rates |

#### 🔹 Dimension Tables
| Table | Description |
|-------|-------------|
| `DimCustomer` | Customer demographics |
| `DimProduct`, `DimProductSubcategory`, `DimProductCategory` | Product hierarchy |
| `DimStore` | Store metadata |
| `DimChannel` | Sales channel (Online/Store) |
| `DimDate` | Calendar |
| `DimGeography` | Location data |
| `DimEmployee` | Sales personnel |
| `DimPromotion` | Promotional campaigns |
| `DimCurrency` | Currency codes |

---

## 🎯 B. Project Goals & Stakeholder Needs
### 1. Scenario
As a **BI Analyst** within the company's IT department, I was tasked with leveraging Power BI to construct reports on various topics, catering to different stakeholders across multiple units. The specific request for this project originated from the Head of Customer Service.

### 2. Manager's Requirements
The Head of Customer Service requested a data transformation and analysis project within Power BI, including charts, graphs, and pivot tables, to provide the following information:

#### a) Customer Retention Analysis (Cohort Analysis)
The Head of Customer Service aimed to understand the number of new customers and the retention rate of online customers across subsequent days or months using a Cohort model. This analysis would inform improvements to increase customer retention.
- Calculate the metric for **the number of new customers** ordering by Day or Month.
- Calculate the metric for **the percentage of new customers** returning to order by Day or Month.
- Create a matrix table (Cohort) displaying both the count of new customers and the percentage of returning customers across two timeframes: daily and monthly.
- Implement slicers for customer country, yearly income, age, occupation, and store to enable detailed filtering.
#### b) Customer Segmentation Analysis (RFM Model)
The Head of Customer Service sought to classify the customer base using an R-F-M (Recency, Frequency, Monetary) model based on online purchase data. This would enable understanding the size and characteristics of each customer segment, facilitating targeted promotional campaigns and customer care programs.
- Calculate total purchase value **(Monetary)**, purchase frequency **(Frequency)**, and time elapsed since the last purchase **(Recency)** for individual customers and the entire customer base.
- Classify customers into distinct groups for management purposes, such as Loyal Customers, Frequent Buyers, General Customers, and Customers Needing Attention.
- Calculate the number of customers within each group and their **demographic** characteristics (e.g., membership level, income, age group, education level, occupation, etc.).
- List a table of all calculated RFM metrics for each customer along with their demographic data.

---

## ⚙️ C. Project Execution
### 1. Data Collection & Understanding
- Downloaded the sample DW from Microsoft.
- Imported data into SQL Server.
- Explored data warehouse schema and relationships.
### 2. Data Preparation
- Connected Power BI to the SQL database
- Used **Power Query** for data cleaning and transformation.
- Built the **data model** linking facts and dimensions.
  ![image](https://github.com/user-attachments/assets/5bbe6368-5124-4d85-a8a6-f865831658b2)

### 3. Data Visualization & Dashboard Design
- Developed pages for:
  - Customer Retention (Cohort Analysis)
  - Customer Segmentation (RFM Model)
- Used visuals:
  - Matrix, Column Charts, Stacked Bar, Gauge, Decomposition Tree
- Enabled interactivity:
  - Bookmarks, Slicers
![image](https://github.com/user-attachments/assets/c2cdd3aa-97a1-4ce1-a5d1-6c67fba5f5ff)

---

## 📈 D. Project Deliverables

### 🔹 Key Insights from Customer Retention Analysis (Dec 2009)
- New Customer Count by Day Matrix: Observing December 5, 2009, Contoso's online stores acquired 373 new customers. However, on the following day, only 6 of them continued to interact and make purchases. When reviewing the overall chart, it is evident that this day marked the most significant loss of newly acquired customers as days passed.
- Customers Coming Back in % by Day Matrix: The most prominent days for customer retention were the 2nd and 3rd days. These days are crucial for customer retention, as after these two days, a continuous decline in customer engagement was observed. From this insight, the customer service department can begin to address the underlying reasons for this trend and implement new measures to prevent it.
Customer Segmentation Analysis (RFM):
### 🔹 Key Insights from Customer Segmentation (RFM)
- Analyzing the RFM scores, the highest Monetary score (3.37) indicates that the average customer spends quite well. However, the lowest Recency score (2.89) suggests a need to actively encourage customers to make new purchases.

---

> 🚀 This project demonstrates end-to-end BI development using Power BI, from data modeling to dashboard storytelling — ideal for roles in Business Intelligence, Data Analysis, and Reporting Automation.
