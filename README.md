# Cryptocurrency Market Analysis

## Project Overview

This project conducts a comprehensive analysis of cryptocurrency market data using K-Means clustering and Principal Component Analysis (PCA). The aim is to segment cryptocurrencies based on price volatility and other market characteristics to better understand the market dynamics.

## Requirements

- Python 3.7+
- Pandas
- hvPlot
- Scikit-learn

## Installation

Install the required packages using the following command:

```bash
pip install pandas hvplot scikit-learn
```

## Usage
To execute the analysis, run the Jupyter Notebook crypto_market_analysis.ipynb after cloning the repository.

## Analysis Steps
- **Data Loading**: Import market data from 'crypto_market_data.csv' and examine its structure and summary statistics.
- **Data Normalization**: Use StandardScaler to normalize the data for clustering analysis.
- **Elbow Method**: Apply the elbow method to determine the optimal number of clusters (k) using both the original and PCA-transformed data.
- **K-Means Clustering**: Perform K-Means clustering on the normalized data and PCA-reduced data.
- **PCA**: Reduce the dataset to three principal components and analyze the explained variance.
- **Visualization**: Visualize clustering results using hvPlot scatter plots.
- **Comparison**: Contrast the results of clustering on the original data with those obtained after PCA using composite hvPlot visualizations.

## Results
- The optimal number of clusters for both the original and PCA data was determined to be 4.
- The explained variance by the three principal components was approximately 89.5%.
- The clustering results indicate clear segmentation of cryptocurrencies based on price volatility over different time horizons.

## Discussion
After analyzing the results, it appears that using PCA to reduce the dimensionality of the data does not significantly impact the clustering outcome. The clusters remain well-defined, suggesting that the principal components retain essential market characteristics.
