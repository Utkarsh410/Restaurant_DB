# Restaurant Orders Data Analysis (SQL)

## Project Overview
This project involves a comprehensive analysis of a restaurant's menu and order history using MySQL. The goal was to extract actionable insights regarding menu performance, customer purchasing habits, and revenue drivers.



## Database Schema
The analysis is based on two primary tables:
- **`menu_items`**: Contains item names, categories (American, Asian, Italian, Mexican), and prices.
- **`order_details`**: Contains transaction records including dates, times, and item associations.

## Analytical Objectives
The project is divided into three key areas of focus:

### 1. Menu Analysis
- Identified the total number of dishes and price distributions.
- Conducted a deep dive into specific cuisines (e.g., Italian) to find average pricing and variety.
- **Key Script:** `OBJ_3_menu_analysis.sql`

### 2. Order Volume & Trends
- Analyzed the date range of the dataset to understand business longevity.
- Identified peak order periods and calculated the total number of unique orders.
- Filtered for high-volume orders (more than 12 items) to understand "bulk" purchasing behavior.
- **Key Script:** `OBJ_2_order_trends.sql`

### 3. Customer Behavior & Revenue
- Linked orders to menu items to identify the most and least popular dishes.
- Identified the top 5 highest-spending orders.
- Analyzed the composition of high-value orders to see which categories contribute most to top-line revenue.
- **Key Script:** `OBJ_1_customer_behavior.sql`

## How to Run the Scripts
1. Clone this repository.
2. Run `data/create_restaurant_db.sql` in your SQL editor (like MySQL Workbench) to set up the database and populate it with data.
3. Execute the scripts in the `scripts/` folder to view the analytical results.

## Key Insights
- **Top Revenue Driver:** Order #440 was the highest spend, with a heavy concentration in specific cuisine categories.
- **Inventory Focus:** Identified the least-ordered items, providing a basis for potential menu optimization or removal.
- **Order Density:** Most orders contain a manageable number of items, but a segment of "mega-orders" (12+ items) suggests opportunities for group catering services.
