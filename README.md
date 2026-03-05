



**Merchandise Sales Analysis Dashboard**



**Project Overview**



This project analyzes the performance of merchandise sales for \*\*Lee Chatman\*\*, a popular U.S. influencer with over 7 million TikTok followers who launched his merchandise line in 2023. The goal of this analysis is to understand sales trends, customer behavior, product performance, and geographic distribution of orders using \*\*Power BI\*\*. 



The dashboard provides interactive insights into product performance, customer demographics, ratings, and shipping behavior.





**Dashboard Preview**



**Sales Overview Dashboard**







This page focuses on overall sales performance and key KPIs.



Key metrics include:



\* Total Sales

\* Total Quantity Sold

\* Total Orders

\* Average Rating

\* Shipping Performance



Key visual insights:



\* Monthly sales trends

\* Buyer gender distribution

\* Sales by age bucket

\* Sales by product category

\* Location performance breakdown







**Merchandise Performance Dashboard**







This page dives deeper into product-level performance and customer feedback.



Key insights:



\* Top performing products by sales

\* Product category comparison

\* Sales distribution by rating

\* Customer review analysis

\* Shipping trends by product category



---



**Key Business Questions**



The analysis focuses on answering several important business questions: 



\* What are the overall sales trends?

\* Which product categories perform the best?

\* What are the most and least popular products?

\* How does location affect sales performance?

\* What impact does international shipping have on sales?

\* What is the demographic profile of buyers?

\* How do ratings and reviews correlate with sales?

\* What are the trends in shipping charges?

\* How do discounts or promotional pricing influence purchasing behavior?

\* Are there patterns in repeat purchases?







**Data Sources**



The dataset includes information on:



\* Orders

\* Products

\* Product Categories

\* Customer demographics

\* Shipping details

\* Locations

\* Ratings and reviews



Key tables used in the data model:



\* `SalesFacts`

\* `ProductDim`

\* `LocationDim`

\* `Calendar`



The model follows a \*\*Star Schema\*\*, with fact and dimension tables optimized for Power BI analytics.







Tools Used



\* Power BI Desktop

\* DAX

\* Power Query

\* Data Modeling (Star Schema)

\* GitHub for project documentation







Key Features in the Dashboard



The dashboard includes several advanced Power BI techniques:



\* Time Intelligence (MoM Sales)

\* Custom Tooltip Pages

\* Dynamic Star Rating Visuals

\* Interactive Slicers

\* Drill-through Pages

\* Conditional Formatting

\* REPT() based visual bars

\* SWITCH() based rating logic







Example DAX Measures



Example: Month-over-Month Sales



DAX

MoM Sales =

CALCULATE(

&nbsp;   \[Total Sales],

&nbsp;   DATEADD(Calendar\[Date], -1, MONTH)

)





Example: Star Rating Display



```DAX

Star Rating =

REPT("★", SalesFacts\[Rating]) \&

REPT("☆", 5 - SalesFacts\[Rating])

```







**Project Structure**





Merchandise-Sales-Analysis

│

├── data

│   └── Merchandise Sales Dataset.xlsx

│

├── dashboards

│   └── Lee\_Chatman\_Mine.pbix

│

├── images

│   ├── sales\_overview.png

│   └── merch\_performance.png

│

└── README.md









\# Key Insights



Some insights from the dashboard include:



\* Certain product categories dominate total sales.

\* Sales patterns fluctuate across months with noticeable peaks.

\* Product ratings strongly influence purchasing behavior.

\* Location significantly impacts total order volume.

\* Shipping costs and international orders influence overall sales patterns.







How to Use This Project



1\. Download the `.pbix` file

2\. Open it in \*\*Power BI Desktop\*\*

3\. Interact with slicers and visuals to explore insights

4\. Navigate between dashboard pages







Future Improvements



Potential improvements for this analysis:



\* Customer lifetime value analysis

\* Repeat purchase segmentation

\* Marketing campaign impact analysis

\* Predictive sales forecasting

\* Sentiment analysis on product reviews







Author



John Abah

Data Science \& Analytics



---





