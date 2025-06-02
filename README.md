# Customer Segmentation Based on Credit Card Data

This project focused on customer segmentation to support the development of a more targeted marketing strategy. The dataset includes behavioral data from approximately 9,000 active credit card holders over the past 6 months, containing 18 behavioral features.  
[Link to the Kaggle dataset](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)

## Data Analysis and Preprocessing

Before applying clustering algorithms, a comprehensive exploratory data analysis was conducted:  
- Distribution analysis of numerical features  
- Outlier detection  
- Correlation analysis  
- Investigation of factors affecting clustering quality

## Clustering Methods Used

The following clustering algorithms were tested in the project:  
- **K-Means**  
- **DBSCAN**  
- **BIRCH**

## Visualization of Clustering Results

To visually assess the clustering output, the following plots were created:  
- **Boxplots** to visualize feature distributions within clusters  
- **Barplots** to analyze the mean values of features across clusters  
(Visualized using Seaborn and Matplotlib)

## Statistical Validation of Cluster Differences

To validate the statistical significance of differences between clusters:  
- Features were tested for normality  
- For normally distributed features: One-way ANOVA was applied  
- For non-normal distributions:
  - Mann–Whitney U test (for 2 groups)
  - Kruskal–Wallis test (for 3 or more groups)
- The significance level was set to **α = 0.05**
- Features with statistically significant differences between clusters were identified

## Clustering Results Summary

| Clustering Method    | Number of Clusters | Silhouette Score | Calinski-Harabasz Index |
|----------------------|--------------------|------------------|--------------------------|
| **KMeans**           | 2                  | 0.1880           | 531.35                   |
| **DBSCAN**           | 2                  | 0.2016           | 7.66                     |
| **BIRCH**            | 2                  | 0.4155           | 7.66                     |

---

This approach enabled the identification of meaningful customer segments, providing a solid foundation for personalized marketing strategies.
