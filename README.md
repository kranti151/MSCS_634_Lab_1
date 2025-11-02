# MSCS_634_Lab_1


**Name:** [Komalben Suthar]  
**Course:** MSCS 634 – Data Analysis & Visualization  
**Lab Assignment:** Lab 1 – Data Exploration and Preprocessing

---

## Purpose of the Lab
The goal of this lab was to explore, preprocess, and analyze a real-world dataset of Amazon products. This involved data cleaning, handling missing values and outliers, reducing data dimensions, scaling, discretizing continuous variables, and performing statistical analysis. The lab also focused on creating meaningful visualizations to understand relationships, distributions, and trends in the data.

---

## Key Insights

### Visualizations:
- **Scatter Plot (Discounted Price vs Rating):** No strong linear relationship, indicating price does not always influence ratings.
- **Histogram of Ratings:** Most products have high ratings (4–5 stars), reflecting positive customer feedback.
- **Bar Chart of Categories:** Certain categories, such as Electronics and Home, dominate the dataset.
- **Box Plots:** Highlighted outliers in pricing and rating counts.

### Statistical Measures:
- **Central Tendency:** Mean rating ≈ 4.09, median rating = 4.1, mode = 4.1.
- **Dispersion:** Price-related columns had high variability; rating counts were skewed with many missing values.
- **Correlation Analysis:** Limited correlation among numeric features, indicating variables like price and discount percentage are weakly related to rating.

---

## Challenges and Decisions
- **Missing Values:** Columns like `discounted_price` and `actual_price` were completely missing. Filled numeric values with mean where possible and set missing categories to 'Unknown'.
- **Outliers:** No significant outliers in the reduced dataset after preprocessing.
- **Data Reduction:** Dropped less relevant columns (reviews, links) and sampled 70% of the dataset for faster processing.
- **Scaling & Discretization:** Applied Min-Max scaling to pricing and discount columns; discretized ratings into Low, Medium, High for categorical analysis.
- **Correlation Matrix:** Initially failed due to all-NaN columns; resolved by selecting only numeric columns with valid values.

---

This lab strengthened skills in data cleaning, visualization, and basic statistical analysis while demonstrating how preprocessing decisions affect downstream insights.
