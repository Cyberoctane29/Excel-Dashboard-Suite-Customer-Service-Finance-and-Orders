# Excel Dashboard Suite: Customer Service, Finance & Orders - A Data-Driven Exploration in Dashboard Design

This project is a suite of three interactive Excel dashboards: Customer Service, Finance, and Orders Management, built to showcase how spreadsheet tools can transform raw business data into actionable insights. By combining KPI tracking, time-series analysis, and interactive filtering, the dashboards provide a 360-degree view of a food chain’s operations, covering sales performance, customer satisfaction, and financial trends. The project leverages advanced Excel features such as PivotTables, PivotCharts, Slicers, and Conditional Formatting to deliver clean, user-friendly, and data-driven decision support.

Access the Dashboards

If you’d like to directly explore the interactive dashboards and project files, you can access them here:

[Google Drive link](https://drive.google.com/drive/u/0/folders/11tU4WL2K5XuClsYWiobEU3VvtfNuW4jh) : https://drive.google.com/drive/u/0/folders/11tU4WL2K5XuClsYWiobEU3VvtfNuW4jh

For the complete project details, including dataset context, analysis workflow, and documented insights, continue with this repository.

## **Project Overview**

The **Comprehensive Business Operations Dashboard Suite** project aims to:

* **Monitor Sales Operations**: Track total orders, revenue, average order value, discounts, and product-level performance through the Orders Management Dashboard  
* **Evaluate Customer Experience**: Analyze customer interactions, satisfaction (CSAT) scores, agent efficiency, and workload distribution using the Customer Service Dashboard  
* **Assess Financial Performance**: Examine sales distribution, revenue trends, regional performance, and identify underperforming products with the Finance Dashboard  
* **Enable Strategic Decisions**: Provide stakeholders with a 360-degree view of business operations, turning raw transactional data into actionable insights for optimization and growth  

## **Dataset Structure**

The project is built on three interlinked datasets capturing customer interactions, financial transactions, and order-level details. Together, they provide a holistic view of customer service performance, sales trends, and operational efficiency.  

**Customer Service Dataset:**  
Captures customer support interactions to analyze service quality and agent performance. Key features include:

* `Customer_ID`, `Order_ID`: Unique identifiers linking service tickets to specific customers and orders  
* `Contact_Date`, `Contact_Day`, `Contact_Date_Month`: Temporal details for tracking patterns in service requests  
* `Contact_Type`: Nature of the interaction (e.g., Query, Request)  
* `Is_it_for_an_Order`: Binary indicator specifying whether the contact relates to an order  
* `Ticket_ID`: Unique support ticket reference  
* `Agent_Handled`: Agent assigned to the case  
* `Rating_Given`: Customer satisfaction rating (scale 1–10)  

**Finance Dataset:**  
Tracks financial outcomes of sales transactions to monitor revenue, discounts, and regional performance. Key features include:

* `Order_ID`, `Product_ID`: Transactional identifiers for mapping orders to products  
* `Sale_Date`: Date of purchase  
* `Amount_in_Sales`: Gross sales value  
* `Discounted_Value`: Net revenue after discounts  
* `Region`: Geographical market segmentation (North, South, East, etc.)  

**Orders Dataset:**  
Provides detailed order-level insights for operational analysis. Key features include:

* `Order_ID`, `Product_ID`: Core identifiers linking orders with products  
* `Product_Name`, `Order_Type`: Item description and sales channel (Online vs. Physical Visit)  
* `Price_of_One_Product`: Unit price of the product  
* `Agent`: Staff member responsible for processing the sale  
* `No_of_Products_in_one_Sale`: Quantity purchased in the order  
* `Discount`: Percentage discount applied  
* `Revenue_before_discount`, `Revenue_after_discount`, `Discount_Amount`: Calculated fields for tracking pricing and discount impacts  

This dataset ecosystem enables the creation of three interactive dashboards: Customer Service, Finance, and Orders Management, each highlighting a different dimension of business performance. The integrated view supports data-driven decisions to improve customer experience, optimize sales strategies, and streamline operations.

## **Dashboard Development & Analytical Workflow**

- **Formulated Targeted Business Questions**  
  Defined key operational questions for each dashboard to guide the analysis. For example, in the Orders Dashboard I evaluated the relationship between discount strategy and profitability, while in the Customer Service Dashboard I focused on identifying the root causes of complaints.  

- **Data Preparation & Feature Engineering**  
  - Cleaned and standardized all datasets to ensure accuracy and consistency.  
  - Engineered new calculated fields such as discrete sales buckets (e.g., ₹300–₹500) to analyze purchasing patterns and agent-specific performance metrics like Average CSAT.  

- **Pivot-Based Analysis & Visualization**  
  - Leveraged PivotTables and PivotCharts to aggregate raw data and answer key business questions.  
  - Created time-series trends for daily revenue, broke down CSAT scores by agent and contact type, and compared product-level sales performance.  

- **Interactive Dashboard Construction**  
  - Assembled three distinct dashboards (Orders, Customer Service, Finance), each tailored to its functional audience.  
  - Incorporated slicers for dynamic filtering by Agent, Region, and Order Type.  
  - Applied a clean, minimalist design with a consistent pastel color palette to enhance readability for non-technical stakeholders.  

- **Insight Generation & Reporting**  
  - Synthesized the visual analysis into actionable insights written directly on the dashboards.  
  - Key findings included pinpointing underperforming products (PIZB0005 & PIZB0006), linking order-related issues to customer complaints, and providing a framework to evaluate the ROI of discount strategies on a per-agent basis.  

## **Key Insights**

### **Financial & Product Performance**
- **Underperforming Products**: PIZB0005 (₹10,677 revenue, ₹628 avg. sales) and PIZB0006 (₹5,077 revenue, ₹564 avg. sales) were identified as significant underperformers, signaling candidates for strategic review or discontinuation.  
- **Revenue Concentration**: 73% of sales occur within the ₹500–₹900 range, highlighting this as the core pricing sweet spot and a key segment for retention and upselling.  
- **Volume vs. Value Discrepancy**: While the *Large Paneer Tikka Pizzabun* drove high order volumes, the standard *Paneer Tikka Pizzabun* generated higher total revenue, underscoring the distinction between popularity and profitability.  
- **Sales Trend Decline**: Despite stable average ticket sizes (~₹5,000), overall sales volumes declined after July, reflecting possible product mix shifts or increased discounting pressure.  

### **Customer Service Drivers & Agent Performance**
- **Interaction Mix**: Requests (53%) and Queries (38%) dominate customer contact, while Complaints remain limited (9%).  
- **Non-Order Related Issues**: A substantial portion of queries and complaints are unrelated to orders, indicating friction in pre-sales information and general support.  
- **Agent CSAT Gap**: Satisfaction scores varied, with Adrien Martin (7.3) outperforming peers Albain Forestier and Roch Cousineau (6.9), highlighting training and coaching opportunities.  
- **Service Quality by Contact Type**: Requests achieved the highest CSAT (7.2), compared to Queries (6.9) and Complaints (6.6), showing dissatisfaction is most pronounced in complaint handling.  

### **Operational & Weekly Trends**
- **Order & Revenue Profile**: Across 794 orders, the business generated ₹2,38,246 in revenue with average revenue per order at ₹300.06 and average discount at ₹251.92.  
- **Volatile Daily Sales**: Revenue and order volumes tracked closely but showed sharp, sporadic peaks (late June, mid-July), indicating demand volatility and opportunities for smoothing strategies.  
- **Product Winners & Laggards**: Paneer Tikka and Large Paneer Tikka Pizzabuns each drove over ₹54,000 in revenue, while Aloo Shots Pizzabun lagged at just ₹10,046.  
- **Weekly Customer Trends**: Interactions peaked on Mondays, declined steadily through the week, and CSAT was highest midweek (Wednesday avg. 7.4), suggesting opportunities to optimize staffing and workload distribution.  


## **Project Highlights**

* Developed a **comprehensive suite of three interactive Excel dashboards** (Orders, Customer Service, Finance) to provide a 360° view of business operations  
* Adopted a **question-driven analytical approach**, leveraging PivotTables, PivotCharts, Slicers, and Conditional Formatting to transform raw data into actionable intelligence  
* Engineered **custom KPIs and calculated fields**, including sales buckets, agent-level CSAT, and average revenue per order, to uncover hidden performance drivers  
* Identified **critical business insights** such as the divergence between high-volume vs. high-revenue products, underperforming product lines, and regional sales disparities  
* Implemented a **clean, user-centric design** with interactive filtering and a minimalist pastel theme, ensuring accessibility and clarity for non-technical stakeholders  
* Delivered a **scalable framework for decision-making**, offering insights on staffing optimization, discount strategy ROI, and customer satisfaction improvement  


This project demonstrates how Microsoft Excel can be leveraged to build a cohesive suite of interactive dashboards, transforming raw and siloed operational data into integrated business intelligence that delivers actionable insights and drives strategic decision-making across sales, finance, and customer service operations.

