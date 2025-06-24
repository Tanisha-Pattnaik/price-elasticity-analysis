
Price Elasticity & Promotion Strategy Analysis

This project analyzes the impact of price changes on demand for three categories — Diapers, Breakfast Cereals, and Headphones — using anonymized Amazon sales data (2017–2019). The goal is to optimize promotion strategies using price elasticity estimates and SKU segmentation.

Project Objectives

- Identify sales spikes using 7-day rolling averages
- Segment SKUs into Top, Core, and Tail based on cumulative sales share
- Analyze price evolution across years and categories
- Estimate price elasticity at segment and SKU level
- Recommend promotion strategies backed by statistical analysis

Project Structure

- `notebooks/`: Contains Jupyter Notebook with full analysis
- `presentation/`: Final PPT summarizing insights and recommendations
- `data/`: Sample dataset (with anonymized trends)
- `visuals/`: Plots generated during analysis (optional)

Methodology

Data Exploration (EDA):
Analyzed ASIN-level daily sales and price data from 2017–2019 across three categories: Diapers, Headphones, and Cereals.

Sale Event Detection:
Applied a 7-day rolling average to identify sales spikes indicating promotion periods.

SKU Segmentation:
Classified SKUs into Top, Core, and Tail using cumulative sales contribution (Pareto-based segmentation).

Price Evolution Analysis:
Measured category-level price trends and linked increases to new product introductions vs. price hikes on existing SKUs.

Price Elasticity Estimation:
Used log-log OLS regression to estimate segment-level and SKU-level elasticity.

Insights & Recommendations:
Delivered segment-specific promotion strategies based on elasticity and SKU performance.



Key Insights

- Top SKUs are highly price-sensitive (Elasticity ≈ -0.58)
- Cereal category introduced 200+ new SKUs, driving average price up
- Spikes in sales aligned with typical promotional periods
- Promotions on inelastic Tail SKUs have negligible volume impact

Tools & Techniques

- Python (Pandas, NumPy, Statsmodels, Seaborn, Matplotlib)
- OLS Regression (Log-Log model for elasticity)
- Rolling average smoothing
- SKU segmentation using cumulative share logic

Requirements

```bash
pip install -r requirements.txt

