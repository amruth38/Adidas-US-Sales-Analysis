# Adidas US Sales Analysis

## Table of Contents

1. [Objective](#objective)
2. [Project Highlights](#project-highlights)
   - Key Metrics
   - Analysis Areas
3. [Data Source](#data-source)
4. [Methodology](#methodology)
   - Data Cleaning and Preparation
   - Visualization
   - Analysis
5. [Tools and Technologies](#tools-and-technologies)
6. [Key Insights](#key-insights)
   - Gender Preference Target Audience for Profits
   - Sales Method's Influence on Operating Profits
   - Profit Margins vs Operating Profits
7. [Future Improvements](#future-improvements)
8. [Challenges and Solutions](#challenges-and-solutions)
9. [How to Use](#how-to-use)
10. [Contact](#contact)

## Objective
The goal of this project is to analyze Adidas' sales data to identify key insights that can enhance sales performance and optimize business strategies. This involves exploring trends, uncovering growth opportunities, and understanding customer preferences.

---

## Project Highlights

### Key Metrics
- **Total Sales:** $89,990,212.50
- **Total Profit:** $33,213,476.14
- **Average Price per Unit:** $45.22
- **Total Units Sold:** 2,478,861

### Analysis Areas
1. **Profit by Retailer**  
   - Identified top-performing retailers:
     - **West Gear**: $8,566,787.18
     - **Foot Locker**: $8,072,124.81
     - **Sports Direct**: $7,433,295.96
2. **Sales Trends Over Time**  
   - Tracked sales performance by year, quarter, month, and day.
   - Saw a great improvement in profits from 2021 compared to 2020.
3. **Gender-Wise Product Category Performance**  
   - Units sold by gender:
     - **Female:** 1,143,332 units
     - **Male:** 1,335,529 units
   - Top-selling categories:
     - Women's Apparel: 433,827 units
     - Men's Street Footwear: 593,320 units
4. **Top Performing Cities by Profit**  
   - Top 5 cities:
     - **Charleston**: $1,560,719.01 profit, 44% margin
     - **New York**: $1,389,997.32 profit, 40% margin
     - **Miami**: $1,216,861.91 profit, 43% margin
     - **Portland**: $1,076,079.94 profit, 41% margin
     - **San Francisco**: $1,025,624.96 profit, 36% margin
5. **Strategic Insights**  
   - **Gender Preference:**
     - Balanced profits from male and female categories in Charleston and Portland.
     - Potential to improve in women's apparel in Miami and New York.
   - **Sales Methods:**
     - San Francisco profits mainly from outlets, while Portland and Charleston have balanced streams across methods.
     - Miami lacks outlet sales and has low online performance.
   - **Profit Margins:**
     - Charleston has the best balance between margin percentage and operating profits.
     - New York has the lowest margin despite high sales.

---

## Data Source
The data for this analysis was sourced from [Kaggle - Adidas Sales Dataset](https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset).

---

## Methodology
1. **Data Cleaning and Preparation:**
   - Processed the dataset to calculate total sales, profits, and average price per unit.
   - Created a "gender" column to categorize products based on keywords (e.g., "Women").
2. **Visualization:**
   - Used graphs and charts to represent sales trends and insights.
   - Adjusted axis units and labels for better readability.
3. **Analysis:**
   - Conducted detailed exploration of profitability, customer preferences, and sales patterns.

---

## Tools and Technologies
- **Microsoft Excel:** Data cleaning, Data processing, analysis and visualization.
- **Formulas:**
  - `=IF(ISNUMBER(SEARCH("Women",G2)),"Female","Male")` for gender categorization.
- **Graph Customization:** Adjusted axis to display values in millions.

---

## Key Insights

1. **Gender Preference Target Audience for Profits:**
   - **San Francisco**:
     - Balanced profits from both male and female products, with a slight edge from men's products.
     - Significant opportunity to improve sales in Women’s Apparel, which is currently the lowest-performing category in the city.
   - **Portland**:
     - Equal profit distribution between men’s and women’s products.
     - Opportunity to improve sales in Men’s Apparel, which is the lowest in the top 5 cities.
   - **Miami**:
     - Profits are concentrated in Men’s Street Footwear and Women’s Apparel.
     - Significant gaps in sales for Women's Athletic Footwear and Men’s Street Footwear, indicating areas for growth.
   - **New York**:
     - Strong performance from Men’s Street Footwear and Women’s Athletic Footwear.
     - Opportunity to boost Women's Apparel sales, which is not performing as well.
   - **Charleston**:
     - Balanced gender-wise profit distribution, with strong performances in both Men’s and Women’s Apparel and Men’s Athletic Footwear.
     - Charleston is the top performer in gender-balanced product categories, highlighting its well-rounded market appeal.

2. **Sales Method's Influence on Operating Profits:**
   - **San Francisco**: 
     - Majority of profits come from outlets, with very few from online and no in-store sales. This indicates an opportunity to diversify sales channels.
   - **Portland**: 
     - Profits are well balanced across online, in-store, and outlet channels, reflecting a more diversified and healthy sales strategy.
   - **Miami**: 
     - Lacks outlet sales, with most profits coming from stores. This underutilization of online and outlet channels presents a growth opportunity.
   - **New York**: 
     - Primarily profits from outlets, with fewer profits from stores and online channels. There's potential to boost online and in-store sales.
   - **Charleston**: 
     - A balanced mix of online and in-store sales, with no outlet sales, suggesting that further expansion into outlet channels could be explored.

3. **Profit Margins vs Operating Profits:**
   - **Charleston**: 
     - High operating profit margin that aligns well with overall profits and total sales, indicating a healthy, efficient market strategy.
   - **New York**: 
     - Low operating profit margin despite high total sales, suggesting that improving efficiency or cost management could help boost profitability.
   - **Miami and Portland**: 
     - Both cities exhibit healthier profit margins compared to others, with Miami slightly outperforming Portland in margin.
   - **San Francisco**: 
     - Operating profit margin is relatively low considering its total sales and profits, indicating inefficiencies that need addressing.


---

## Future Improvements
- **Expand Analysis**: Include regional, seasonal trends, and demographic insights to refine targeting.
- **Predictive Modeling**: Forecast future sales and optimize inventory with machine learning.
- **Refine Strategies**: Tailor city and retailer-specific sales strategies based on insights.

---

## Challenges and Solutions

1. **Data Cleaning and Transformation**:
   - **Problem**: Inconsistent descriptions and missing values.
   - **Solution**: Use `=TRIM()`, `=SUBSTITUTE()`, `=CLEAN()` to clean data. For blanks, use `=IF(ISBLANK(A2), "N/A", A2)`.

2. **Creating a Multi-Axis Chart**:
   - **Problem**: Difficult to create a chart with three axes (Average Operating Profit Margin vs Operating Profits vs Cities).
   - **Solution**: 
     - Create a Combo Chart: Select Data → Insert → Combo Chart → Custom Combination.
     - Assign Average Operating Profit Margin to the secondary axis.
     - Set Operating Profit to the primary axis and use cities for the horizontal axis.
     - Adjust axis scales and chart types (Column for Operating Profits, Line for Profit Margin).
    
3. **Sales Trend Analysis at Different Levels**:
   - **Problem**: Difficult to analyze trends by year, quarter, month.
   - **Solution**: Create PivotTable → Group by Date → Insert PivotChart for trend analysis.

4. **Formatting Sales Graph Axis to Display in Millions**:
   - **Problem**: Unable to change axis to display sales in millions.
   - **Solution**: Right-click on axis → Format Axis → Display Units → Millions.

5. **Categorizing Products by Gender**:
   - **Problem**: Need to specify product gender.
   - **Solution**: Add “gender” column. Use formula `=IF(ISNUMBER(SEARCH("Women", G2)), "Female", "Male")`.

6. **Visualizing Profit Margins by City**:
   - **Problem**: Difficulty comparing profit margins.
   - **Solution**: Create scatter plot with profit margins on one axis and total sales on the other.

7. **Dynamic Chart Updates**:
   - **Problem**: Charts not updating with new data.
   - **Solution**: Use Excel Tables for auto-updating charts: Select Data → Insert → Table → Format as Table.

---

## How to Use
1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset).
2. Follow the methodology outlined above to replicate the analysis.
3. Explore the findings and insights to understand Adidas US sales performance.

---

## Contact
For any questions or feedback, feel free to reach out via the repository's Issues section.
