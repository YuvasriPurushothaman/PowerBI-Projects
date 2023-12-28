# Saled Dashboard

### Dashboard Link : [https://app.powerbi.com/groups/me/reports/35ae63c8-7139-4a39-b6ed-bc956a00d0fd/ReportSection?experience=power-bi](https://app.powerbi.com/groups/me/reports/35ae63c8-7139-4a39-b6ed-bc956a00d0fd/ReportSection?experience=power-bi)

## Problem Statement

The task at hand involves the creation of a comprehensive sales dashboard leveraging a dataset containing essential information on sales transactions. The dataset encompasses key columns including RowID, OrderID, OrderDate, Sales, CustomerName, City, Country, Market, ProductID, Category, SubCategory, Profit, and Year. The primary objective is to design an interactive dashboard offering insights into critical performance indicators related to sales operations. The dashboard should provide an overview section featuring total sales revenue, total profit, and the net profit. Sales trends over time should be visually represented, allowing users to customize time ranges. Geographical analysis should include a map showcasing sales distribution across different countries and cities. Customer insights are crucial, necessitating the identification of top shipping mode and a breakdown of sales on a basis of segment. Similarly, the dashboard should offer insights into sales performance, highlighting the most sold SubCategory by segment. Profitability analysis, yearly comparisons, and interactive filters for market segments and time periods should also be incorporated. The ultimate goal is to deliver a user-friendly, visually engaging dashboard that empowers stakeholders to derive actionable insights from the sales dataset. The chosen data visualization tools should facilitate dynamic exploration and analysis, ensuring accessibility for end-users.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : For calculating the total sales sum up the sales column.
- Step 6 : For calculating the net profit % a measure is created.
- Step 7 : Various visuals are created to derive a insight from data.
- Step 8 : Visual filters (Slicers) were added for four fields named "Year" & "Market".
- Step 9 : Map visual were added to the canvas for determining market wise sales.
           


Snap of Total sales card visual ,

![Totalsales_card](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/a4810aa3-ad46-4f76-a434-b0e446712a38)

        
New measure was created to find Net Profit %.

Following DAX expression was written for the same,
        
        PROFIT % = (SUM('Global-Superstore'[Profit])/SUM('Global-Superstore'[Sales]))*100
A card visual was used to represent Net Profit.

![Netprofit_card](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/db619670-c18d-4ba2-b772-df9137dbcfd7)


 A card visual was used to represent the number of distinct products and Total shipping cost.
 

![Disproductcard](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/9d5d9cde-93c2-4194-a407-838645eb44df)

 
    
 A Line and Clustered column chart visual was used to represent this Sales by year.
 
 
 
![Salesbyyear](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/cba4d0e0-f1d1-43b9-9ee5-47330950834e)

 A Pie chart is used to represent Segment wise sales.
 

![segmentwise sales](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/7bc4c5aa-68eb-486a-bf7c-08e4f6c4d685)

A Filter which uses market column to filter the all other visuals.

![filterbymarket](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/9f56efaa-0821-4d57-814c-9cb221d7ea8f)

# Snapshot of Dashboard (Power BI Service)

 ![full](https://github.com/YuvasriPurushothaman/PowerBI-Projects/assets/97823980/b8413005-2b2e-48a6-a426-55174fc087d2)


### INSIGHTS
  
  (a) Sales Increase Year-wise

  (b) Shipping Mode Usage by Country
  
  (c) Net Profit
  
  (d) Year-wise Percentage of Profit on Sales
  
  (e) Total Cost Involved in Shipping
  
  (f) Most Sold Sub-category

  (g) Segment Consuming More Sales
  
  (h) Total Sales over Years
  
  (i) Sales Range with Respect to Market

  #### (a) Sales Increase Year-wise
The sales is increased over every year and Calculating the percentage of profit on sales for each year provides a profitability ratio. This insight helps evaluate the efficiency of converting sales into profit, offering a nuanced understanding of financial performance.

#### (b) Shipping Mode Usage by Country
A predominant inclination towards standard shipping is observed globally, with a notable preference evident across all countries compared to alternative shipping methods.

#### (c) Net Profit
The net profit has exhibited consistent annual growth, increasing by a minimum of 0.40% each year. However, an exception occurred in 2014, where there was a notable decline of 0.22%. This deviation can be attributed to the higher shipping costs incurred in 2014 compared to other years, impacting the overall profitability for that specific period.

#### (d) Year-wise Percentage of Profit on Sales
The standard annual profit increment of 0.40% was deviated from in 2014, as a substantial decrease of 22% was recorded for that particular year. 

#### (e) Total Cost Involved in Shipping
The higher shipping costs incurred in 2014 compared to other years.

#### (f) Most Sold Sub-category
Binders, Storage and art reign supreme as the top-selling subcategory, outpacing competitors with its unmatched sales performance.

#### (g) Segment Consuming More Sales
Within the consumer, corporate, and home office segments, the consumer segment notably emerges as the primary driver of sales, demonstrating its preeminent position in the market.

#### (h) Total Sales over Years
The cumulative sales figure of 12.64 million over the past four years serves as a benchmark and encourages us to set an ambitious yet achievable target for the next period. This performance metric not only reflects our past success but also provides a strategic point of reference to guide our efforts towards surpassing this milestone in the upcoming business cycle. With a clear understanding of our historical performance, we can leverage this achievement to propel our sales trajectory to new heights.

#### (i) Sales Range with Respect to Market
Leveraging map visualization through a bubble chart to represent sales in relation to the market is a strategic approach that will empower us to pinpoint areas where our performance may be lagging. This visual representation allows for a comprehensive assessment, with each bubble indicating a specific market. The size of the bubbles corresponds to the sales volume, enabling a quick and insightful analysis of relative performance across diverse markets. This tool not only facilitates the identification of underperforming markets but also guides targeted strategies to address and improve our market presence in those areas.



  


