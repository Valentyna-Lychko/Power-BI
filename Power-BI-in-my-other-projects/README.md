
# Power BI: Integration with API to Create a Dashboard

---

## Working with Supermarket Sales Data

- Various functions were used to calculate and aggregate the data.
- Different types of visualizations were developed to analyze supermarket sales data.

---

## Project Description

This project demonstrates the process of creating an interactive dashboard in Power BI with API integration. The primary goal is to ensure automatic data loading from external sources, its transformation, and visualization in a user-friendly format.

- The data was analyzed using Kaggle's "Supermarket Sales" dataset.

---

## Dataset Description

The **"Supermarket Sales"** dataset contains information about items, sellers, and customers who conducted transactions in the supermarket over a certain period.  
It enables the exploration and analysis of various aspects of sales, such as product popularity, customer behavior, and sales dependency on dates.

---

## Data Analysis

- Analyzed sales based on key indicators, including revenue, average item price, and the number of items sold.
- Developed interactive visualizations to examine changes over time, product categories, and payment methods.
- Added filters to improve data analysis convenience by year and month.

---

## Working with External API

- Integrated the National Bank of Ukraine API ([bank.gov.ua](https://bank.gov.ua)).
- Retrieved the USD exchange rate for the latest date.
- Used the Power BI WEB connector to load the USD exchange rate.

### Data Sources:

1. National Bank of Ukraine - [bank.gov.ua](https://bank.gov.ua)  
2. Open Data - [bank.gov.ua/ua/open-data/api-dev](https://bank.gov.ua/ua/open-data/api-dev)  
3. Official exchange rates of the hryvnia to foreign currencies and accounting prices of bank metals (JSON format).  

---

## Working with Data in Power BI

- Developed charts and visualizations, including time series, bar charts, and pie charts for data analysis.
- Calculated measures for key metrics (total revenue, average item price, etc.).
- Added a new "Currency" table with two rows: UAH and USD.
- Included a "Currency" single-selection filter in the dashboard for currency conversion.
- Implemented automatic changes in chart values based on currency selection via DAX formulas.

---

### DAX Formulas Used:

#### Average Price:
```DAX
IF(
    MAX('Currency'[Currency]) = "UAH",
    AVERAGE('supermarket_sales - Sheet1 (2)'[Unit price]) * SUM(USD[rate]),
    AVERAGE('supermarket_sales - Sheet1 (2)'[Unit price])
)
```

#### Total by Currency:
```DAX
IF(
    MAX('Currency'[Currency]) = "UAH",
    SUM('supermarket_sales - Sheet1 (2)'[Total]) * SUM(USD[rate]),
    SUM('supermarket_sales - Sheet1 (2)'[Total])
)
```

- These measures were applied to the charts.

---

## Completed

- Created a file in Power BI Desktop.  
- Built 6 visual components on a single slide.  
- Integrated external API.  
- Implemented a currency conversion mechanism using a parameter.

---

## Implementation Details

### Data Calculations:

- Calculated total revenue for each sales month.
- Built a line chart to visualize this data.
- Calculated the average price of items for each category.
- Created a bar chart to display this data.

### Sales Visualization:

- Built a time series chart to analyze sales changes over time.
- Added filters by year and month.
- Created a bar chart to analyze the number of units sold in each product category.
- Implemented stacking to display product distribution by months or locations.
- Built a pie chart to analyze sales by payment methods.

### Working with External API:

- Integrated the National Bank of Ukraine API.
- Retrieved the USD exchange rate for the latest date.
- Used the Power BI WEB connector to load the USD exchange rate.
- Created a new Currency table (via Enter Data) with two rows: UAH and USD.
- Added a Currency single-selection filter to the dashboard.
- Implemented currency conversion for charts using DAX formulas.

---

## Repository Files:

- **[Dashboard.pbix](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboards/Sales_Analysis_with_Currency_Conversion.pbix)**  
  The main Power BI file containing implemented visualizations and analytics.  


---

This project helps enhance Power BI skills by creating analytical solutions based on real data.  

Other projects using tools such as Tableau, Looker Studio, SQL, and BigQuery can be found in the **[Data-Analytics-Projects](https://github.com/Valentyna-Lychko/Data-Analytics-Projects/tree/main/Dashboard_Images)** repository.

---
