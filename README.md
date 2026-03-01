![Project-logo](https://github.com/isachenko-andrii/E-commerce-sales-analysis/blob/main/Project-logo.png)
<div align="center">  
    
# E-Commerce Sales Performance Dashboard<br>(Looker Studio)  
  
</div>
  
## Project Overview  
  
This project is dedicated to the analysis of retail sales of an online store. The goal is to visualize key performance indicators (KPIs), identify trends in product categories, and analyze the geography of orders for management decision-making.

[Link to interactive dashboard](https://lookerstudio.google.com/u/0/reporting/77b746a6-39e8-41c2-bacc-51662ee9b358)  

**Technology Stack**
  
**Visualization Tool:** Google Looker Studio
**Data Source:** [CSV Dataset (E-commerce transactions)](https://drive.google.com/file/d/1crbddZ7lr0ttwX_F0QUdKdPO7z__XojU)  
**Analysis Types:** EDA, Time Series, Geospatial Analysis, Category Segmentation.  
  
## Stages of project implementation
The dashboard development process was divided into 5 key stages:

**1. Defining business goals and KPIs** 
  
At the first stage, the questions that the dashboard should answer were formulated:  
 * **What is the revenue dynamics by month?**
 * **Which product categories bring the greatest profit?**
 * **How are orders distributed by geography and device types?**
 * **What percentage of orders are successfully delivered, and what percentage are returned or canceled?**  
  
**2. Data Preparation and Cleaning**  
  
Before importing into Looker Studio, the data was checked for quality:  
 * **Typification:** Converting the order_date column to a date format for correct time series construction.
 * **Validation:** Checking the price, quantity, and discount columns for anomalous values.
 * **Creating calculated fields:** Calculating total values ​​(Total Revenue) taking into account discounts, if this was not provided in the raw data.
   
**3. Designing the dashboard architecture**  
  
I developed a logical structure of the page for user convenience (UI/UX analytics):  
 * **Top level:** Key figures (Scorecards) for a quick overview of the state of affairs.
 * **Middle level:** Trends (Time Series) and categorical breakdown (Pie/Bar Charts).
 * **Bottom level:** Drill-down by geography and operational status.  
  
**4. Visualization and development**  
  
Configuring Looker Studio tools:  

 * Creating interactive filters (by date, country, category) for deeper drilling into the data (Drill-down).
 * Configuring the color scheme for quick visual distinction of order statuses (e.g. green for "Delivered", red for "Cancelled").

**5. Analysis of results and formulation of insights**  
  
The final stage is the interpretation of graphs:
 * Identification of correlation between device type and average check.
 * Analysis of the effectiveness of payment methods in different regions.
 * Preparation of recommendations for optimizing marketing efforts in countries with low AOV.
   
## Key metrics and visualizations  
 
The dashboard is divided into logical blocks that allow you to evaluate your business from different perspectives:  

**1. Key indicators (Scorecards):**  
 * **Total Revenue:** Total sales.
 * **Total Orders:** Number of transactions processed.
 * **Average Order Value (AOV):** Average check.  
  
**2. Discount Impact: Analysis of the impact of discounts on the final amount.**  

Sales dynamics (Time Series):

A line graph that displays revenue fluctuations by date, allowing you to identify seasonality and peak sales days.

**3. Category and product analysis:**  
 * Sales distribution by category (Electronics, Home, Toys, Books, Clothing).  
 * Top products by revenue and number of orders.  

**4. Geography and customer behavior:**  

 * **Device Usage:** Analysis of devices from which purchases were made (Mobile, Desktop, Tablet).  
 * **Payment Methods:** Breakdown by payment method (Credit Card, PayPal, COD).  

**5. Operational metrics**  
 * Delivery status (Delivered, Shipped, Pending, Returned, Cancelled), which is critical for logistics and churn analysis.

## Data structure  
  
The dataset used contains the following fields:  
 * **order_id, user_id:** <code>Order and user identifiers.</code>
 * **order_date:** <code>Transaction date.</code>
 * **category:** <code>Product category.</code>
 * **price, quantity, discount:** <code>Price, quantity and discount percentage.</code>
 * **total:** <code>Total order amount.</code>
 * **payment_method, delivery_status:** <code>Operational data.</code>
 * **country, device:** <code>Segmentation features.</code>

## Key Insights  
 * **Category Popularity:** The Electronics and Home categories show the highest average order value.
 * **Mobile Traffic:** A significant portion of orders are placed on mobile devices, indicating the need to optimize for a mobile-first experience.
 * **Logistics:** High levels of Cancelled and Returned statuses in certain regions require additional attention to service quality or product descriptions.

## Visualizations  

  

## How to use  

 * Review the ecommerce_dataset.csv file to understand the structure.
 * Follow the link to Looker Studio to interact with filters (date, country, category).

## Contact  
    
**Name:** [Andrii Isachenko](https://isachenko-andrii.github.io)    
**LinkedIn:** [Andrii Isachenko](https://www.linkedin.com/in/isachenko-andrii/)  
**E-mail:** isao.datastudio@gmail.com   
  
## Acknowledgments    
  
 - Thanks to the [Data Analyst/GoIT](https://goit.global/ua/courses/data-analytics/) course, which was part of this project.  
  
---
  
**Project Status:** Completed.
    
**License:** MIT License.  
