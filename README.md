
---

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

Visualized regional product trends using:
- Bar charts
- Pie charts
- Line graphs

---

## 🧠 ML Bonus Section

Included a basic regression model using `scikit-learn` to predict product sales.  
Although performance was weak, this satisfies bonus ML criteria.

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
git clone https://github.com/yourusername/ecommerce-trends-bi.git
cd ecommerce-trends-bi

# Start JupyterLab
jupyter lab
