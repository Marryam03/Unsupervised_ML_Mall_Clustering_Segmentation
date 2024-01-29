This code uses a dataset on mall customers to perform customer segmentation through various clustering algorithms. The process involves exploratory data analysis, visualization, and clustering using K-means, Hierarchical Clustering, DBSCAN, and Mean Shift.

**1. Data Exploration:**
   - The dataset contains information about customers, including age, annual income, spending score, and gender.
   - No missing values are present in the dataset.
   - The skewness of the 'Annual Income' and 'Age' columns indicates right-skewed distributions.

**2. Data Visualization:**
   - Line plots, count plots, violin plots, and pair plots are used to visualize relationships and distributions.
   - Heatmaps and scatter plots explore correlations and patterns between features.

**3. Clustering:**
   - **K-means:**
      - The Elbow method and Silhouette Score help determine the optimal number of clusters (k=5).
      - Visualizations show well-segmented clusters for 'Annual Income vs Spending Score.'

   - **Hierarchical Clustering:**
      - Dendrogram analysis suggests 5 clusters.
      - Visualization reveals clusters based on 'Annual Income vs Spending Score.'

   - **DBSCAN:**
      - Epsilon and min_samples are tuned to achieve meaningful clusters.
      - Outliers are identified.

   - **Mean Shift:**
      - Bandwidth is selected using `estimate_bandwidth()` function.
      - Clusters and centroids are visualized.

**4. Model Evaluation Metrics:**
   - Silhouette Score and Davies-Bouldin Score are used for model evaluation.
   - K-means, Hierarchical Clustering, and Mean Shift show relatively higher Silhouette Scores compared to DBSCAN.
   - Davies-Bouldin Scores indicate good cluster separation for all algorithms.
