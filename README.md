# BALAJI-FAST-FOOD-SALES

### Project Overview
This excel project aims to provide insights into the sales performance of the Balaji Fast food reastaurant. By analyzing various aspect of the sales data, i seek to identify trends, make data recommandations and deeper understanding of the company's sales.

### Data Sources
The dataset used for this project is the "Balaji Fast Food Sales.csv" file containing detailed information about each sale made by the reastaurant.

### Tools
- MS Excel - Data cleaning
- SQL Server Management Studio - Data analysis
- PwerBI - Reports and data visualization

### Data cleaning and preparation process
Data was prepared and cleaned thoroughly by performing followingtasks:
1. Danda loading
2. Deleting duplicates
3. Handling missing values
4. Data formatting

### Exploratory Data analysis
Data exploration to answer key questions such as;
- How is the restaurant performance in revenue?
- What are the best and worst selling items?
- What are the total orders placed per day or monthly?
  
### Data analysis
Includes interesting code features such as:
```sql
 SELECT item_name, CAST( SUM(item_price)*100/ (SELECT sum(item_price) FROM BalajiFastFoodSales) AS decimal(10,2)) AS Item_Name_Percent
FROM BalajiFastFoodSales
GROUP BY item_name
Order BY Item_Name_Percent DESC
```

### Results and Findings
 1. The company's revenue is high with a notieable peak on  Weekends and Wednesday.
 2. Sandwich and Frenkies seems to be the best selling items on the menu.
 3. May is the month that sells the most.
 4. Panipuri seem to be the least orderd item on the menu.
 5. Vadapav contributes the least on the revenue.

### Recomandations
Based on the results i would the recomend the following to the owner of the Balaji restaurant:
- He/she must prioritize promoting her items on weekends in order to maximize the revenue.
- The focus of the makerting should on the sandwich and frenkie which are the customers' favourites.
- The owner must conduct reviews on why Panipuri is not selling much.

### References
 For dataset: https://www.kaggle.com/datasets/rajatsurana979/fast-food-sales-report


