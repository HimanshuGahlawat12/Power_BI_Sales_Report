# Power_BI_Sales_Report
Power BI dashboard to analyze the sales data.

**Overview**
This GitHub repository houses the codebase and project artifacts for a comprehensive Sales Report project. The project aims to gather and analyze sales data, create insightful visualizations, and present key findings through a one-page Dashboard. The Business Requirement Document (BRD) serves as the foundation for the project, outlining data sources, tasks, and objectives.

**Project Structure**
**1. Data Gathering / Requirement**

**1.1 Sales Data Sources**
**Sales (folder by year):** Contains yearly sales data files.
**Categories (Excel):** Product categorization.
**Geography (Excel):** Geographical data.
**Product (CSV / Database):** Product details.
**SalesRep (Excel):** Sales representatives data.
**SubCategories (Excel):** Subcategories information.

**1.2 Task 1.1 - Sales Fact Table Loader Mechanism**
Implemented a robust mechanism to load files from the sales folder into a single Sales fact table.
Resilient to file removals and automatically loads new yearly sales files upon refresh.

**2. Data Modeling**
**2.1 Task 2.1 **- Sales Fact Table Transformations
Split Country from City in the "Location" field, setting up correct data types for Geo maps.
Updated Date field format for proper date setup.
**2.2 Task 2.2 - **Create GeoKey
Established a unique key (GeoKey) in Sales and Geography tables.
**2.3 Task 2.3 -** Clean ID Columns
Implemented a function to remove the "ID - " part from certain ID columns in SalesRep and SubCategory queries.
**2.4 Task 2.4 -** Create Data Model
Connected all tables to create a comprehensive Data Model, utilizing the Calendar table set up in the Power BI file (pbix).

**3. DAX Calculations**
**3.1 to 3.7 - Various DAX Measures**
Calculated Total Revenue, Total Cost, Gross Profit, MoM Growth Change%, and AVG Sales per day, and conducted a Breakdown Analysis by Product.
Implemented specific time measures like QoQ Growth for the Quarterly Business Report (QBR).
**4. Dashboard Creation**

Utilized Power BI for data cleaning and visualization.
Employed SQL for connecting to the data source.
Presented final analysis in a PowerPoint presentation.
