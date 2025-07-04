# AI-ML-Task8

1. Import Libraries

> These libraries help with:

     > Data handling (pandas, numpy)
     > Visualization (matplotlib, seaborn)
     > Machine learning and clustering (KMeans, StandardScaler, silhouette_score)

2. Load Dataset

> Loads the dataset into a DataFrame.
> It includes customer data like Gender, Age, Income, and Spending Score.

3. Feature Selection

> Only selects the numeric features relevant for customer behavior.
> These features reflect how much a customer earns and how much they spend — perfect for segmentation.

4. Feature Scaling

> Standardization converts values to have zero mean and unit variance.
> This ensures both features contribute equally during distance calculation in K-Means.

5. Visualize Scaled Data

> Plots the scaled income vs. spending to visually inspect any natural groupings or patterns.

6. Elbow Method to Find Best K

> Tries different cluster numbers (K=1 to 10).
> Calculates WCSS (within-cluster sum of squares) for each K.
> Elbow point in the plot shows the best value of K (where improvement slows down).

7. K-Means Clustering (K=5)

> K-Means is applied with K=5 (chosen from elbow method).
> Each customer is assigned to one of the 5 clusters.
> A new column Cluster is added to the original data.

8. Cluster Visualization

> Displays customer groups in different colors.
> Cluster centroids are shown using red 'X' markers.
> Helps understand which clusters are high/low income or spending.

9. Silhouette Score

> Measures how well-separated the clusters are.
> Score closer to 1 = better clustering, 0 = overlapping clusters, < 0 = bad clusters.

