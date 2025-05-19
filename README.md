# Crypto Clustering Analysis

## Overview
This project implements an unsupervised machine learning approach to analyze and cluster cryptocurrencies based on their price change percentages over different time periods. The analysis helps identify patterns and group similar cryptocurrencies together, which can be valuable for portfolio management and investment strategies.

## Project Structure
```
CryptoClustering/
├── Crypto_Clustering_starter_code.ipynb  # Jupyter notebook with the analysis
├── README.md                             # This file
└── Resources/
    └── crypto_market_data.csv          # Cryptocurrency price change data
```

## Technologies Used
- Python 3.8+
- Jupyter Notebook
- Pandas - Data manipulation and analysis
- scikit-learn - Machine learning algorithms
  - KMeans - For clustering
  - StandardScaler - For feature scaling
  - PCA - For dimensionality reduction
- Matplotlib - For data visualization

## Dataset
The dataset (`crypto_market_data.csv`) contains the following price change percentage features for various cryptocurrencies:
- price_change_percentage_24h
- price_change_percentage_7d
- price_change_percentage_14d
- price_change_percentage_30d
- price_change_percentage_60d
- price_change_percentage_200d
- price_change_percentage_1y

## Analysis Steps
1. **Data Loading and Preprocessing**
   - Load the cryptocurrency market data
   - Clean and prepare the data for analysis
   - Scale the data using StandardScaler

2. **Finding Optimal Number of Clusters**
   - Use the Elbow method to determine the optimal number of clusters
   - Plot the inertia values to visualize the optimal k value

3. **K-Means Clustering**
   - Apply K-Means clustering with the optimal k value
   - Analyze the resulting clusters

4. **Dimensionality Reduction with PCA**
   - Reduce the features to 3 principal components
   - Apply K-Means clustering to the PCA-transformed data

5. **Visualization and Analysis**
   - Create visualizations to compare clustering results
   - Analyze the differences between original and PCA-reduced clustering

## Key Findings
- The Elbow method suggested [X] as the optimal number of clusters for this dataset
- The clusters group cryptocurrencies with similar price change patterns
- Dimensionality reduction with PCA helped [describe impact on clustering]

## How to Run
1. Ensure you have Python 3.8+ installed
2. Install the required packages:
   ```
   pip install pandas jupyter scikit-learn matplotlib
   ```
3. Open the Jupyter notebook:
   ```
   jupyter notebook Crypto_Clustering_starter_code.ipynb
   ```
4. Run all cells to execute the analysis

## Results
[Include key visualizations or summary statistics from your analysis]

## Future Work
- Experiment with different clustering algorithms (DBSCAN, Hierarchical, etc.)
- Incorporate additional cryptocurrency features
- Implement real-time data streaming for up-to-date analysis

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Dataset provided by [source if applicable]
- Built as part of [course/program name if applicable]