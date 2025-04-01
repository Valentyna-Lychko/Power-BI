# Pizza Sales Analysis

---

## Dashboard Description

### General Overview:
This dashboard is designed to analyze pizza sales, catering to the interests of both pizzeria owners and customers. It consists of four pages, each providing unique insights for better understanding of key business aspects. Each page includes navigation buttons for easy switching between tabs.

### Dashboard Pages:
- **Overview** - Pizza Business Performance: Trends and Key Metrics
- **Sales** - Revenue, Orders, and Quantity Analysis
- **Price** - Pizza Pricing by Size and m²
- **Leaders** - Top Pizzas by Size, Price, and Popularity

The data for analysis was sourced from Kaggle, processed in Power Query. Measures were calculated in DAX, and a parameter was added to enhance dashboard interactivity.

![](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboard_Images/Pizza_All.png)

---

## Detailed Page Descriptions:

### Overview - Pizza Business Performance: Trends and Key Metrics
This section provides a general overview of the business, including key sales metrics and main trends. The charts on the page illustrate changes in revenue, orders, and pizza quantities over time.

#### Key Elements:
- **Cards with key metrics:**
  - Total Revenue
  - Total Orders
  - Total Quantity
  - Average Check
  - Average Price
  - Number of Pizzas
- **Combo Chart – "Revenue & Orders by Month":**
  - Bars show total revenue by month.
  - The line represents the total number of orders.
  - No significant seasonal fluctuations observed.
- **Bar Chart – "Total Quantity by Size & Category":**
  - Displays the distribution of sold pizza quantities by category and size.
  - Highest demand for pizzas:
    - Classic pizza size S.
    - Vegetarian and chicken pizza size L.
- **Area Chart – "Average Orders Per Day Week":**
  - Peak is on Friday, lowest orders on Sunday.
- **Area Chart – "Average Orders Per Hour Per Day":**
  - Most orders occur at 6 PM, fewest during morning hours.

![](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboard_Images/Pizza_Overview.png)

---

### Sales - Revenue, Orders, and Quantity Analysis
This section provides detailed information on sales by pizza categories and sizes.

#### Key Elements:
- **Horizontal Bar Chart – "Orders by pizza_category":**
  - Shows the number of orders across different pizza categories.
- **Sankey Diagram – "size → category → name":**
  - Visualizes the distribution of orders by pizza sizes.
- **Horizontal Bar Chart – Pizza rankings by order count.**
- **Toggle Buttons (Revenue, Orders, Quantity):**
  - Switch the analytic parameter on the dashboard.

![](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboard_Images/Pizza_Sales.png)

---

### Price - Pizza Pricing by Size and m²
This section focuses on pizza pricing by size and compares pizza prices by area.

#### Key Elements:
- **Table – "The price of pizza by size":**
  - Displays prices of pizzas in different sizes.
- **Treemap – "Median price per m²":**
  - Visualizes the median price of pizzas per square meter.

![](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboard_Images/Pizza_Price.png)

---

### Leaders - Top Pizzas by Size, Price, and Popularity
This section presents the rankings of pizzas leading in various criteria.

#### Key Elements:
- **Tables:**
  - Most Popular Pizza.
  - Min Priced Pizza.
  - Big Pizza.
- **Treemap – "Promising pizzas":**
  - Highlights pizzas to watch out for.
- **Table – "Pizza Sizes":**
  - Details about pizza sizes and areas.

![](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboard_Images/Pizza_Leaders.png)

---

## Additional Features:
- Each page of the dashboard includes navigation buttons for quick tab switching.

---

## Project Files:

- **Power BI File**  
[Pizza_Sales_Analysis.pbix](https://github.com/Valentyna-Lychko/Power-BI/blob/main/Dashboards/Pizza_Sales_Analysis.pbix):  
Download for a detailed view of the interactive dashboard.

- **Video Demonstration:**  
Watch the video to see the interactivity and functionality of the dashboard: [Pizza Sales Analysis - Video](https://github.com/Valentyna-Lychko/Power-BI-UA/blob/main/Dashboard_Videos/Pizza_video.mp4)

---

## Conclusions and Recommendations:
This dashboard enables detailed analysis of pizzeria sales performance, identifies the most popular items, and optimizes pricing strategies.

### Recommendations:
- **Menu Optimization:** Use data from the "Sales" section to identify the most popular types of pizzas.
- **Pricing Strategy:** Analyze data from the "Price" section to adjust pizza prices.
- **Staff Optimization:** Use graphs from the "Overview" section to plan staff schedules (peak sales time: Friday at 6 PM).

These recommendations aim to enhance business efficiency and improve sales through Power BI analytics.

---


