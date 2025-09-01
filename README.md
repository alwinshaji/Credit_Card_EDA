# Credit Card Fraud Analysis

This repository contains exploratory data analysis (EDA) on a **Credit Card Fraud Detection** dataset sourced from Kaggle. The dataset includes 8 features that represent customer behavior, transaction characteristics and fraud labels.

## Dataset Overview

- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/dhanushnarayananr/credit-card-fraud)
- **Features**:
  - `distance_from_home`
  - `distance_from_last_transaction`
  - `ratio_to_median_purchase_price`
  - `repeat_retailer`
  - `used_chip`
  - `used_pin_number`
  - `online_order`
  - `fraud` (target label)

## Project Workflow

1. **Data Exploration & Cleaning**  
   - Loaded the data and examined its structure (shape, data types, missing values).

2. **Univariate & Bivariate Analysis**  
   - Generated summary statistics (mean, median, quartiles).  
   - Visualized distributions using boxplots, histograms, and KDE plots to compare fraud vs non-fraud patterns.

3. **Outlier & Anomaly Detection**  
   - Used IQR-based calculations to count outliers in each feature.  
   - Identified potential fraud signals in high-value or unusual transactions.

4. **Feature Correlation Analysis**  
   - Computed correlations between features and fraud, visualized with heatmaps and bar charts.  
   - Key signals identified: purchase price ratio, online transaction flag, and geographic features.

5. **Dimensionality Reduction with PCA**  
   - Applied Principal Component Analysis to visualize transaction patterns in 2D.  
   - Explored cluster separation between fraud and legitimate transactions.

6. **Insight Synthesis**  
   - Developed clear, actionable insights:
     - Fraud is more likely in transactions that are far from home, far from the last purchase, and have abnormal price ratios.
     - Online purchases carry higher fraud risk, while chip and PIN usage reduce it.
     - Fraudulent transactions exhibit distinct distribution patterns in KDE and PCA visualizations.

## Usage

1. Clone this repository.
2. Run the Jupyter notebook(s) provided.
3. Follow the analysis—starting from loading the data, through visualization, outlier detection, and PCA.
4. Use the insights as a foundation for building predictive or anomaly detection models.

---
