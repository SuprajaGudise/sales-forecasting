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
- Exploring data science and machine learning through sales forecasting projects.
- Check out my [GitHub Stats](https://github.com/SuprajaGuDise) for more insights!

## Stats
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=SuprajaGuDise&show_icons=true)
![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=SuprajaGuDise.sales-forecasting)

More submissions will be added soon!

<body>
  <h1>📈 Sales Forecasting Visualizations</h1>
  <p>Below are key visualizations from the SP25 Sales Forecasting project, showcasing model performance and data trends:</p>

  <h3>Feature Importance </h3>
  <div class="center">
    <img src="https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/PLOT1.jpeg" alt="Feature Importance" class="plot-img" onerror="this.nextElementSibling.style.display='block';">
    <p class="fallback" style="display:none;">Image failed to load. Please check if PLOT1.jpeg exists in the images folder or verify the URL: https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/PLOT1.jpeg</p>
  </div>
  <p>This plot displays the feature importance for the XGBoost model , highlighting key predictors such as Prev_Quarter_Sales, PMI_Lag1, and RevenueGrowth_Diff that significantly influenced sales forecasts, contributing to a test MAE of 627.21.</p>

  <h3>Predicted vs Actual Sales </h3>
  <div class="center">
    <img src="https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/PLOT2.jpeg" alt="Predicted vs Actual" class="plot-img" onerror="this.nextElementSibling.style.display='block';">
    <p class="fallback" style="display:none;">Image failed to load. Please check if PLOT2.jpeg exists in the images folder or verify the URL: https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/PLOT2.jpeg</p>
  </div>
  <p>This scatter plot compares predicted sales against actual sales, demonstrating the model’s ability to capture sales trends across 75 companies, with most points clustering near the diagonal line, indicating good predictive accuracy (test MAE 627.21).</p>

  <h3>Time Series Plot</h3>
  <div class="center">
    <img src="https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/TIMESERIES%20PLOTS.jpeg" alt="Time Series Plot " class="plot-img" onerror="this.src='https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/TIMESERIES_PLOTS.jpeg'; if(this.complete && this.naturalHeight === 0) this.nextElementSibling.style.display='block';">
    <p class="fallback" style="display:none;">Image failed to load. Please check if TIMESERIES PLOTS.jpeg exists in the images folder (may need to rename to TIMESERIES_PLOTS.jpeg) or verify the URL: https://github.com/SuprajaGuDise/sales-forecasting/raw/main/images/TIMESERIES%20PLOTS.jpeg</p>
  </div>
  <p>This time series plot illustrates actual sales (Q1-Q7) alongside the linear regression predictions, highlighting the model’s ability to capture seasonal trends across quarters, though it struggles with sharp fluctuations due to its linear nature.</p>

  
