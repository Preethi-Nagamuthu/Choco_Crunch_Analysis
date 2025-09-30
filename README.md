# Choco_Crunch_Analysis
You’re a Data Analyst at a nutrition research firm analyzing the global chocolate market. The goal is to extract chocolate product data from OpenFoodFacts API, clean and transform it, enrich with derived nutrition metrics, store it in a SQL database, perform EDA and SQL-based insights, and visualize findings via dashboards.
# 📥 Dataset Collection
Extract chocolate product data using:

https://world.openfoodfacts.org/api/v2/search?categories=chocolates&fields=code,product_name,brands,nutriments&page_size=100&page=1

Fetch up to 12,000 records (approx) using pagination.
Extract columns:
 product_code, product_name, brand, and nutriments fields

 # 🛠️ Data Exploration and  🧹Cleaning 
Explore the dataset for missing values.

Identify columns with null values and handle them appropriately.

Drop columns with excessive nulls if necessary.

Impute or manage missing values in other columns based on data type and relevance.

 # 🛠️ Step 3:  Feature Engineering
 sugar_to_carb_ratio → Calculate the ratio between total sugar and total carbohydrates for each product. Useful for identifying products disproportionately high in sugars.

calorie_category → Classify products into 'Low', 'Moderate', or 'High Calorie' groups based on their energy content per 100g.

sugar_category → Similar to calorie category, classify products based on their sugar content per 100g into 'Low Sugar', 'Moderate Sugar', or 'High Sugar' tiers.

is_ultra_processed → Flag products as 'Yes' if their nova-group classification indicates ultra-processed (usually a value of 4); otherwise 'No'.

# 🧮 Exploratory Data Analysis (EDA) with Python
Bar charts to show the number of products in each calorie_category or sugar_category.

Pie charts to illustrate the proportion of products in each nova-group.

Histograms for distribution of calories, sugars, or sugar-to-carb ratio.

Box plots to visualize the spread and outliers of calories or sugar across different brands.

Scatter plots to explore relationships like calories vs. sugars.

Heatmaps to visualize correlations between different numerical nutritional values.

Top N bar plots for brands with highest average calories or sugars.

# 🗃️ SQL Table Design
Table 1: product_info
Table 2: nutrient_info
Table 3: derived_metrics

# 📊 Power BI Visualization 
<img width="1121" height="628" alt="image" src="https://github.com/user-attachments/assets/ee218a2f-9f22-494f-8466-700d0eea47d1" />




