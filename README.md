# Adidas US Sales Analysis

## Table of Contents
- [Objective](#objective)
- [Project Highlights](#project-highlights)
  - [Key Metrics](#key-metrics)
  - [Analysis Areas](#analysis-areas)
- [Data Source](#data-source)
- [Methodology](#methodology)
- [Tools and Technologies](#tools-and-technologies)
- [Key Insights](#key-insights)
- [Challenges and Solutions](#challenges-and-solutions)
- [Future Improvements](#future-improvements)
- [How to Use](#how-to-use)
- [Contact](#contact)


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
- Charleston leads in profitability with a well-balanced gender-wise profit distribution.
- West Gear is the top retailer, followed by Foot Locker and Sports Direct.
- Opportunities to boost women's apparel sales in multiple cities.
- Profitability varies significantly based on sales methods, with some cities underutilizing online and outlet channels.

---

## Challenges and Solutions
1. **Challenge:** Formatting sales graph axis to display in millions.  
   **Solution:** Adjusted axis settings in Excel (`Right Click > Format Axis > Display Units > Millions`).
2. **Challenge:** Categorizing products by gender.  
   **Solution:** Used a formula to identify "Women" products and classify accordingly.

---

## Future Improvements
- Expand analysis to include regional and seasonal trends.
- Incorporate machine learning models to predict future sales trends.
- Optimize retailer-wise sales strategies for better profit margins.

---

## How to Use
1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/heemalichaudhari/adidas-sales-dataset).
2. Follow the methodology outlined above to replicate the analysis.
3. Explore the findings and insights to understand Adidas US sales performance.

---

## Contact
For any questions or feedback, feel free to reach out via the repository's Issues section.
