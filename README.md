# Cryptocurrency Market Analysis Project

## Project Overview

This project involves analyzing cryptocurrency market data to uncover patterns and groupings among various cryptocurrencies. Using data preprocessing, normalization, K-means clustering, Principal Component Analysis (PCA), and visualization techniques, we aim to identify meaningful clusters within the market and understand the influence of various market behaviors on these clusters.

## Data Source

The dataset used in this project is `crypto_market_data.csv`, which includes historical price change percentages over different time frames (24h, 7d, 14d, 30d, 60d, 200d, 1y) for various cryptocurrencies.

## Methodology

### Data Preprocessing and Normalization
- Loaded the market data into a Pandas DataFrame.
- Normalized the data using `StandardScaler` to ensure that the clustering algorithm does not get biased by the scale of the data.

### Clustering with K-means
- Determined the optimal number of clusters (`k`) using the Elbow method by plotting inertia and identifying the point of inflection.
- Applied K-means clustering with the optimal `k` to group cryptocurrencies based on their market behaviors.

### Dimensionality Reduction with PCA
- Conducted Principal Component Analysis (PCA) to reduce the dimensionality of the data while retaining most of the variance.
- Identified the weights of each feature on the principal components to understand their influence.

### Visualization
- Visualized the clusters using scatter plots to illustrate how cryptocurrencies are grouped based on their 24-hour and 7-day price changes.
- Used PCA-reduced data for clustering and visualized the results to compare with the original clustering.

## Key Findings

- The optimal number of clusters identified was `k=4` using the original data and `k=5` with PCA-reduced data, indicating slight differences in cluster structures depending on the dimensionality reduction.
- PCA revealed that certain features have a stronger influence on the principal components, helping to interpret the underlying factors driving market behavior patterns.
- Visualization of clusters provided insights into the market dynamics and how cryptocurrencies relate to each other based on their price change percentages.

## Conclusion

This project showcased the utility of machine learning techniques such as K-means clustering and PCA in analyzing and interpreting complex datasets like cryptocurrency market data. Through this analysis, we gained insights into the clustering of cryptocurrencies based on market behavior, which could be useful for investors, analysts, and enthusiasts interested in the crypto market.
