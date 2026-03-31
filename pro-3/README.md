### Project Name: Sales \& Regional Performance Analysis (Advanced DAX)



#### Project Overview



* The objective of this project is to perform a comprehensive analysis of an e-commerce dataset using Power BI and Advanced DAX. The project focuses on Data Modeling, Calculated Columns, Measures, and Time Intelligence functions to derive actionable business insights.



#### Data Architecture:-



* The following tables from the dataset were utilized to build the star schema model:
* Fact Tables: Sales\_ Fact, Returns\_ Fact.
* Dimension Tables: Customer\_ Dim, Product\_ Dim, Date\_ Dim, Region\_ Dim.



#### Steps \& Tasks Performed :-



1\. Data Transformation (Calculated Columns):

To enhance the analytical depth, specific calculated columns were added to the Fact and Dimension tables:

Profit: Calculated as \[Sales Amount] - \[Cost] within the Sales\_ Fact table.

Return Flag: Implemented logical IF conditions to categorize transactions as "Returned" or "Not Returned".

Customer Full Name: Created by concatenating the First and Last names in the Customer\_ Dim table.

Region Code: Used text manipulation functions (UPPER and LEFT) to generate standardized 3-letter codes for regions.



2\. Measure Management:

A dedicated "Key Measures" table was created to centralize and organize all DAX calculations:

Core Metrics: Total Sales, Total Cost, and Total Profit.

Return Rate: Calculated the percentage of items returned relative to total sales.

Average Sale per Transaction: Derived using the AVERAGEX iterator for transaction-level accuracy.



3\. Quick Measures \& Time Intelligence:

Advanced time-based calculations were implemented to track business growth over time:

MoM Sales Difference: Calculated the variance between the Current Month and the Previous Month's sales.

YoY Sales Growth %: Measured the year-over-year percentage increase in sales.

Sales YTD: Utilized the TOTALYTD function to track cumulative sales from the start of the year.



4\. Advanced Filter Context:

Complex business scenarios were addressed using CALCULATE, ALL, and FILTER functions:

Total Sales (All Regions): Applied the ALL function to ignore regional filters, enabling the calculation of regional contribution percentages.

High Sales Only: Used the FILTER function to aggregate totals specifically for transactions exceeding a $500 threshold.



5\. Advanced Logic \& Iterators:

Sales Status (SWITCH): Developed a dynamic categorization measure to label regions as "High", "Medium", or "Low" based on sales performance.

Iterator Functions: Leveraged SUMX and AVERAGEX for row-level logic and aggregated metrics.



6\. Data Joining (RELATED):

Integrated data across the model using the RELATED() function in the Sales\_ Fact table to pull necessary attributes from Dimension tables for row-level calculations.



##### Output Requirements :-



* In accordance with the project constraints, all analytical results are presented exclusively in a Matrix Visual:
* Hierarchical Grouping: Data is grouped by Region, Month, Product Category, and Customer Segment.
* Constraint: No other visualization types were used to ensure a clean, focused, and professional reporting structure.



#### Skills Learned :-



* Data Relationship Modeling (Star Schema Design).



* Advanced DAX Programming (Calculated Columns vs. Measures).



* Time Intelligence and Trend Analysis.



* Filter Context Manipulation and Row-level Iteration logic.

