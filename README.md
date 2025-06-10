## 🔄 ETL Pipeline

**Extract**: Loaded a regional e-commerce product dataset from CSV  
**Transform**: Cleaned missing values, standardized column names, converted currencies  
**Load**: Stored cleaned data in a local SQLite database (in JupyterLab)

---

## 🧪 Analysis & Insights

- Tracked regional product trends  
- Built a predictive sales model (Linear Regression)  
- Evaluated using:  
  - Mean Squared Error (MSE): 353,196.01  
  - R² Score: -0.02  

> ⚠️ The model underperformed, likely due to lack of key features and non-linear relationships. Still, it demonstrates a complete ML evaluation workflow.

---

## 📊 Dashboard

The dashboard visualizes key regional product trends and insights using the following interactive charts:

- **Stacked Bar Chart**: Displays the sum of sales by category, allowing clear comparison of sales volume across multiple product categories. Categories like "Bedsheets" and "Art and Crafting" show higher total sales, while "Bath and Body" appears among the lower-performing.
  
- **Line Chart**: Shows the sum of sales by year, specifically highlighting sales for 2023 (approx. 276). This visualization helps reveal temporal trends and overall performance.

- **Scatter Chart**: Focuses on the "Makeup" category, comparing metrics such as sum of discounts and sum of sales. This helps identify how pricing strategies (e.g., discounts) impact sales within the category.

- **Clustered Custom Chart**: Compares average price and average rating across different categories. It highlights customer satisfaction versus pricing — for example, categories that are highly rated yet lower priced.

- **Map Visualization**: Shows total sales distribution across cities, with top locations including San Francisco, Phoenix, and Atlanta. Colored points represent product category presence, enabling regional product popularity analysis.

These visualizations offer actionable insights into category performance, pricing effectiveness, customer preferences, and regional demand patterns.

---

## 🧠 ML Bonus Section

Included a basic regression model using `scikit-learn` to predict product sales.  
Although performance was weak, this satisfies bonus ML criteria.

---

## 📅 Task Scheduler & Data Simulation

- The pipeline uses a window task scheduler to automate daily runs.  
- Since the dataset from Kaggle is static, the scheduler generates **synthetic daily data** for 2025 based on patterns from the 2024 data.  
- This synthetic data is used to test ETL processing, alerts, ML predictions, and dashboard updates, simulating a "live" environment without requiring new real data.

---

## 📂 Data Source & Ingestion

- **Source**: Kaggle dataset "Exploring E-commerce Trends" by Muhammad Roshan Riaz  
- **Period Covered**: January 2023 to December 2024  
- **Storage**: Cleaned data saved in local SQLite database in JupyterLab  
- **Simulation**: Synthetic daily data for 2025 is generated based on 2024 patterns to enable continuous testing of pipeline components and ML models.

---

## ⚙️ Technologies Used

- Python (Pandas, Matplotlib, Scikit-learn)  
- SQLite (in JupyterLab)  
- Jupyter Notebooks  
- GitHub for version control  

---

## 📜 How to Run

```bash
# Clone the repo
git clone https://github.com/ShaleenM-cpu/ecommerce-etl-project.git
cd ecommerce-trends-bi

# Start JupyterLab
jupyter lab
