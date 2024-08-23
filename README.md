# Cryptocurrency Clustering Project

## Project Overview
This project focuses on the analysis and clustering of cryptocurrency data using K-Means clustering and Principal Component Analysis (PCA). The objective is to group cryptocurrencies based on their market performance and evaluate the impact of using different numbers of features in clustering.

## Dataset
The data used for this project is a CSV file containing various market metrics for different cryptocurrencies. Key features include:
- Price change percentage over 24 hours (`price_change_percentage_24h`)
- Price change percentage over 7 days (`price_change_percentage_7d`)
- Other relevant market metrics

## Project Steps
1. **Data Loading and Preprocessing:**
   - Load the cryptocurrency market data into a Pandas DataFrame.
   - Normalize the data using `StandardScaler` from scikit-learn.
   
2. **Data Visualization:**
   - Plot the data to understand the distribution and trends.

3. **K-Means Clustering:**
   - Perform K-Means clustering on the scaled data.
   - Use the Elbow method to determine the optimal number of clusters (`k`).
   - Initialize and fit a K-Means model with the optimal `k` value.
   - Predict clusters and add them to the DataFrame.

4. **Principal Component Analysis (PCA):**
   - Reduce the data to three principal components using PCA.
   - Analyze the explained variance to determine how much information is captured by each component.
   - Perform K-Means clustering on the PCA-transformed data.
   
5. **Visualization of Clusters:**
   - Create scatter plots to visualize the clusters in the original and PCA-transformed data.
   - Compare the results to understand the impact of dimensionality reduction.

6. **Analysis of Results:**
   - Evaluate the impact of using fewer features by comparing the clusters formed using the full dataset and the PCA-transformed dataset.

## Conclusion
The project demonstrates how dimensionality reduction techniques like PCA can be used to simplify the clustering process while retaining essential information. The comparison of clusters formed with full and reduced features offers insights into the trade-offs between model complexity and interpretability.

## Requirements
- Python 3.x
- Pandas
- scikit-learn
- hvPlot
- Holoviews

## Running the Project
1. Clone the repository.
2. Ensure you have the required Python libraries installed.
3. Run the Jupyter notebook to reproduce the analysis and visualizations.

## References
- [https://www.mathworks.com/help/stats/kmeans.html
ii