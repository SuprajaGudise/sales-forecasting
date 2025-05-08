# Sales Forecasting

This repository contains code for sales forecasting submissions, showcasing my work on predictive modeling.

<h1 align="center">🌟 Sales Forecasting Repository 🌟</h1>

<p align="center">
  <img src="./images/zbra-marketing-IryWX_OSgh4-unsplash.jpg" alt="Sales Forecasting Banner" width="800">
</p>

<p align="center">
  This repository contains code for sales forecasting submissions, showcasing my work on predictive modeling. Let’s dive into the world of data science! 📈✨
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Made%20with-Jupyter-orange?style=flat-square&logo=jupyter" alt="Jupyter">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
</p>
<h2>Introduction</h2>
<p>The SP25 Sales Forecasting Kaggle Challenge predicts quarterly sales for a steel manufacturer serving 75 customers in Auto, Metal Fabrication, and Infrastructure industries. Accurate forecasts prevent overproduction or shortages, boosting profitability.</p>
<ul>
  <li><strong>Business Impact</strong>: Guides production scheduling, inventory management, resource allocation, and financial planning.</li>
  <li><strong>Model Goal</strong>: Cuts waste, ensures reliable delivery, stabilizes finances, and supports growth.</li>
  <li><strong>Metric</strong>: Mean Absolute Error (MAE), targeting &lt;500 (~10-15% of avg. sales: 3,500).</li>
  <li><strong>Top Model</strong>: XGBoost Regressor (Test MAE 627.21) with target-encoded features, lagged economic indicators, and TimeSeriesSplit validation.</li>
</ul>

<h2>Data Description</h2>
<h3>Overview</h3>
<p>The dataset includes:</p>
<ul>
  <li><code>train.csv</code>: 525 rows (75 companies, Q1-Q7, with Sales).</li>
  <li><code>test.csv</code>: 150 rows (Q8-Q9, for prediction).</li>
  <li><code>sample_submission.csv</code>: Format with ID, Sales.</li>
  <li><code>EconomicIndicators.csv</code>: 28 months of macroeconomic data.</li>
</ul>

<h3>Purpose</h3>
<p>Merges firm-level (e.g., QuickRatio) and macroeconomic (e.g., PMI) data to forecast sales, capturing company and economic trends.</p>

<h3>Key Features</h3>
<table>
  <tr>
    <th>Feature</th>
    <th>Type</th>
    <th>Description</th>
    <th>Relation to Sales</th>
  </tr>
  <tr>
    <td>Company</td>
    <td>Categorical (75)</td>
    <td>Customer name</td>
    <td>Varies by customer</td>
  </tr>
  <tr>
    <td>Quarter</td>
    <td>Categorical (Q1-Q9)</td>
    <td>Sales quarter</td>
    <td>Seasonal impact</td>
  </tr>
  <tr>
    <td>QuickRatio</td>
    <td>Numeric</td>
    <td>Liquidity ratio</td>
    <td>Higher values boost sales</td>
  </tr>
  <tr>
    <td>RevenueGrowth</td>
    <td>Numeric</td>
    <td>Projected growth</td>
    <td>Drives sales</td>
  </tr>
  <tr>
    <td>PMI</td>
    <td>Numeric</td>
    <td>Purchasing Managers Index</td>
    <td>Values &gt;50 increase sales</td>
  </tr>
  <tr>
    <td>Sales</td>
    <td>Numeric</td>
    <td>Quarterly sales (target)</td>
    <td>Target variable</td>
  </tr>
</table>

<h3>Statistics</h3>
<ul>
  <li><strong>Sales</strong>: Mean 3517.12, median 3041, right-skewed, max 11686.</li>
  <li><strong>QuickRatio</strong>: Mean 1.62, near-normal, min 0.50.</li>
  <li><strong>InventoryRatio</strong>: 20.19% missing, median 3.47, right-skewed.</li>
  <li><strong>PMI</strong>: Cyclical, 46.20-59.20.</li>
</ul>

<h3>Insights</h3>
<ul>
  <li>Sales skewness suggests log-transformation.</li>
  <li>InventoryRatio needs median imputation.</li>
  <li>Cyclical indicators require lagged features.</li>
  <li>Use target encoding for Company, one-hot for Region/Industry.</li>
</ul>

## Best Kaggle Submission
- **File**: `submission_23.ipynb`
- **Description**: My top-performing sales forecasting model from Kaggle
- **Dependencies**: See `requirements.txt` for required Python libraries.
- **How to Run**:
  1. Clone the repository: `git clone https://github.com/SuprajaGuDise/sales-forecasting.git`
  2. Install dependencies: `pip install -r requirements.txt`
  3. Place the required datasets (`train.csv`, `test.csv`, `EconomicIndicators.csv`) in the `data` directory. Contact me for access to the datasets.
  4. Run the notebook: `jupyter notebook kaggle_best_submission.ipynb`

## About Me
- I’m a passionate data science and machine learning enthusiast, currently diving deep into sales forecasting projects to uncover actionable insights from complex datasets.
- With a focus on predictive modeling, I enjoy leveraging tools like Python, Pandas, Scikit-learn, and visualization libraries (Matplotlib, Seaborn) to build robust solutions for real-world problems, such as forecasting quarterly sales for a steel manufacturing company.
- Beyond coding, I’m dedicated to continuous learning—whether it’s experimenting with new algorithms, exploring time-series analysis, or staying updated on industry trends in data science.
- Check out my [GitHub Stats](https://github.com/SuprajaGuDise) to see my contributions, or explore my repositories to discover more projects on data analysis, machine learning, and forecasting!

## Stats
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=SuprajaGuDise&show_icons=true)
![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=SuprajaGuDise.sales-forecasting)

More submissions will be added soon!

<body>
  <h1>📈 Sales Forecasting Visualizations</h1>
  <p>Below are key visualizations from the SP25 Sales Forecasting project, showcasing model performance and data trends:</p>

  <h3>Sales Trend by Top 5 Companies</h3>
  <p align="center">
    <img src="https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/sales_trends_top_companies.png" alt="Sales Trends for Top 5 Companies Over Quarters" class="plot-img" onerror="this.nextElementSibling.style.display='block';">
    <p class="fallback" style="display:none;">Image failed to load. Please view the repository’s images folder for 'sales_trends_top_companies.png'.</p>
  </p>
  <p>This plot tracks sales over quarters for the top 5 customers, revealing distinct patterns like Customer A’s consistent high sales and Customer B’s seasonal peaks. It guides customer-specific forecasting by highlighting trends and variability critical for the steel company’s quarterly predictions.</p>

  <h3>Feature Importance Bar Plot</h3>
  <p align="center">
    <img src="https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/feature_importance.png" alt="Feature Importance for Sales Prediction" class="plot-img" onerror="this.nextElementSibling.style.display='block';">
    <p class="fallback" style="display:none;">Image failed to load. Please view the repository’s images folder for 'feature_importance.png'.</p>
  </p>
  <p>This bar plot ranks features like InventoryRatio and QuickRatio as top drivers of sales, based on a Random Forest model. It informs model development by focusing on key factors like inventory and liquidity for accurate sales predictions.</p>

  <h3>Box Plot of Sales by Quarter</h3>
  <p align="center">
    <img src="https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/sales_by_quarter_boxplot.png" alt="Sales Distribution by Quarter" class="plot-img" onerror="this.nextElementSibling.style.display='block';">
    <p class="fallback" style="display:none;">Image failed to load. Please view the repository’s images folder for 'sales_by_quarter_boxplot.png'.</p>
  </p>
  <p>This box plot shows sales distributions across quarters, with Q1 often having higher medians and outliers, indicating seasonal demand spikes. It helps in forecasting by providing insights into quarterly trends and variability for the steel company.</p>
</body>
