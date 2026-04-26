# Ung-dung-hoc-may-phan-cum-tai-san-dau-tu-tren-ro-co-phieu-VN30
📌 Overview

This project applies Big Data and Machine Learning techniques to cluster stocks in the VN30 index based on risk-return characteristics, aiming to support portfolio diversification and investment decision-making.

The study combines:

Financial data analysis
Feature engineering
Dimensionality reduction
Unsupervised learning (Clustering)
🎯 Objectives
Cluster VN30 stocks into meaningful groups based on:
Return
Risk (Volatility)
Sharpe Ratio
Liquidity
Compare ML-based clustering with traditional industry classification
Propose investment strategies based on clustering results
📊 Dataset
Source: Yahoo Finance API (yfinance)
Scope:
30 stocks from VN30 Index
Time range: 01/01/2022 – 01/01/2026
Features:
Price (Adjusted Close)
Volume
Fundamental indicators:
P/E
P/B
Market Cap
Beta
⚙️ Methodology
1. Data Collection
Use yfinance to extract historical stock data
Collect both:
Time series data
Fundamental data
2. Data Preprocessing
Handle missing values:
Forward Fill (ffill)
Backward Fill (bfill)
Replace missing fundamental values with median
Normalize data using Z-score
3. Feature Engineering

Key features extracted:

Return (annualized)
Volatility (standard deviation)
Sharpe Ratio
Liquidity
4. Dimensionality Reduction
Apply PCA (Principal Component Analysis)
Reduce feature space to 2–3 dimensions for clustering & visualization
5. Clustering
Algorithm: K-Means
Optimal number of clusters:
Determined using:
Elbow Method
Silhouette Score
Final choice: k = 3
6. Visualization
PCA scatter plot
Radar Chart (cluster characteristics)
Boxplot (distribution analysis)
Heatmap (comparison with traditional classification)
