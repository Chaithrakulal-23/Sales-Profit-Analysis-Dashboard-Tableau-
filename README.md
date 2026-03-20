# Sales & Profit Analysis Dashboard (Tableau)

### Dashboard Link : https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/e06f69a38a0026e9216c6a6faf791454d6ce7c07/TableauDASHBOARD1.twb
## Problem Statement

This dashboard helps analyze sales, profit, and order performance across different regions and customer segments. It enables better understanding of how profit is distributed, how much each region contributes to overall sales, and how order quantity changes over time.

The dashboard also highlights the relationship between sales and profit, helping identify high-revenue but low-profit customers.

---

### Steps followed 

- Step 1 : Loaded the Sample Superstore dataset into Tableau, where the Orders table contains 8,399 rows.

- Step 2 : Reviewed all columns to understand the dataset and ensure data consistency.

- Step 3 : Created a calculated field to group data based on Unit Price into categories A, B, and C.
          
       Grouping based on Unit Price =
         if(airline_passenger_satisfaction[Age]<=25, "0-25 (25 included)",
        
        if(airline_passenger_satisfaction[Age]<=50, "25-50 (50 included)",
        
        if(airline_passenger_satisfaction[Age]<=75, "50-75 (75 included)",
        
        "75-100 (100 included)")))
  ![Snap_1](https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/7dc8835aac8930aa7a022cc5e3723f5c0d317005/TAB1.png)

Snap of new calculated column ,

![Snap_1](https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/af71c07f06a59fdc3255891bcbfbe9cb43f178f7/TABD1.1.png)

- Step 4 : Applied the Unit Price Group field as a filter across all charts for dynamic analysis.

- Step 5 : In the first sheet, created a bar chart to represent Profit by Region and Customer Segment. Applied color based on customer segment and added labels for better visualization.
![Snap_1](https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/9459b1ca1d79ff9b0fa32995a0f96d1564db0ef9/bar-d1.png)
- Step 6 : In another sheet, created a pie chart to represent Percentage Sales Contribution and Sales by Region using sum of sales and region-based coloring, along with percentage labels.
![Snap_1](https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/4d809b6964d6b732f91a35a109c92126a6d54ebf/pie-d1.png)
- Step 7 : Created a line chart to represent Order Quantity by Month using order date and sum of order quantity.
![Snap_1](https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/168dcbd995927751bf2c9df644199f3b028cd902/line-d1.png)
- Step 8 : Built a scatter plot to analyze the relationship between Sales and Profit, using customer name in the detail shelf to show individual data points.
![Snap_1](https://github.com/Chaithrakulal-23/Sales-Profit-Analysis-Dashboard-Tableau-/blob/5ceef51e6ef08f01b94420255a8eb54090e53224/scatter-d1.png)
- Step 9 : Designed a dashboard by combining all visuals and formatted it properly.

- Step 10 : Enabled interactivity by applying filters so that all charts are connected and respond dynamically to user selections.

---

# Snapshot of Dashboard

![Snap_1](https://user-images.githubusercontent.com/102996550/174089602-ab834a6b-62ce-4b62-8922-a1d241ec240e.jpg)
---

# Insights

A single dashboard was created using Tableau to analyze sales and profit data.

### [1] Profit Analysis
- Profit varies across regions and customer segments
- Some segments contribute more profit within specific regions

### [2] Sales Contribution
- Different regions contribute differently to total sales
- Certain regions dominate overall sales percentage

### [3] Order Trends
- Order quantity fluctuates across months
- Helps identify peak and low sales periods

### [4] Sales vs Profit Relationship
- Some customers generate high sales but low profit
- Indicates potential areas for cost optimization

### [5] Unit Price Segmentation
- Products are grouped into categories (A, B, C) based on price
- Helps in analyzing performance across pricing segments
