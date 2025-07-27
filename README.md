# Credit card Weekly Transaction Report

# Project Objectives:
 To develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends, enabling stakeholders to monitor and analyzw credit card opetations effectively. 

# Dashboard Overview

The Power BI dashboard provides visualizations and insights into:

- Revenue trends across quarters and weeks
- Spending behavior by:
  - Education level
  - Income group
  - Age group
  - Gender
  - Card category
- Revenue and interest earned by customer job types
- Top-performing states and usage types (swipe, chip, online)

# Steps Involved While Making the Project

1. Data Preprocessing
   - Downloaded the weekly credit card transaction dataset.
   - Cleaned and formatted the data using Excel:
     - Converted date format from `DD-MM-YYYY` to `YYYY-MM-DD` using the `TEXT()` function.
     - Ensured consistency in column names and data types.

2. Database Creation (MySQL)
   - Created a new MySQL database with two main tables: `customers` and `credit card transactions`.
   - Imported the cleaned dataset into MySQL using import tools.

3. Power BI Integration 
   - Connected Power BI to the MySQL database.
   - Established relationships between the tables for data modeling.

4. Data Modeling in Power BI 
   - Created calculated columns using DAX:
     - `Age Group` based on customer age
     - `Income Group` for income segmentation
   - Developed DAX measures such as:
     - `Total Revenue`
     - `Interest Earned`
     - `Total Transaction Amount`

5. Dashboard Development 
   - Designed a multi-page, interactive dashboard featuring:
     - KPIs (Total Revenue, Transactions, Interest, Customer Count)
     - Slicers for quarter, gender, and card category
     - Bar/line charts segmented by job, education, marital status, etc.
   - Applied filters for better user experience.

6. Data Update: Week 53 Ingestion
   - After the initial dashboard was completed, an additional Week 53 dataset became available.
   - Imported the new Week 53 data into the MySQL database.
   - Refreshed the Power BI data source to automatically update all visuals and calculations, reflecting the most recent data.

7. Deployment
   - Exported and shared the final `.pbix` report as a PDF in this repository.
   
 Tools & Technologies Used

- Power BI Desktop
- MySQL for relational data modeling
- DAX (Data Analysis Expressions) in Power Bi Desktop
- Excel for data cleaning

# Project Insights:
 
Overview Year-To-Date:
- Overall revenue is 57 Million
-Total interest is 8 Million
- Total transaction amount is 46 Million
- Male customers are contributinng more in the revenue i.e 31 Million
- Blue & Silver cards are contributing to 93% of overall transactions
- Texas(TX), New York(NY) & California (CA) is contributing to 68% 
- Overall Activation rate is 57.5%
- Overall Delinquent rate is 6.06%

Week Over Week Change: Week 53
- Revenue increased by 28.8%
- Total Transaction amount increased by 35.04%
- Total transaction count increased by 3.39%
