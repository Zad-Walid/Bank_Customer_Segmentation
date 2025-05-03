# Bank_Customer_Segmentation & Product Recommendation

##  Overview
This project focuses on segmenting bank customers using unsupervised learning techniques and recommending personalized bank products or investment plans based on customer profiles.

## Dataset
- **Source**: Internal bank dataset
- **Original_Data_Set**: 1048567 record
- **Cleaned_Data_Set**: 657,829 customer-level aggregated records
- **Columns include**:
  - Demographics: `CustomerAge`, `CustGender`, `CustLocation`
  - Account features: `CustAccountBalance`, `BalancedCategory`
  - Product holdings: `Product_*`
  - Transaction behavior: `AvgTransactionAmount`, `TotalTransactions`

## Objectives
- Clean and preprocess transaction-level data.
- Engineer meaningful customer-level features.
- Apply multiple clustering algorithms to segment customers.
- Interpret clusters and generate tailored product recommendations.

##  Technologies Used
- **Python** (NumPy, pandas)
- **scikit-learn**
- **K-means** , **HDBSCAN**, **DBSCAN**, **GaussianMixture**
- **TruncatedSVD**, **t-SNE**
- **Google Colab**

##  Feature Engineering
- Encoded categorical features 
- Scaled numerical features
- Reduced dimensionality
- Create new features that are more representitive to the models

##  Clustering Models
- **KMeans** – baseline clustering
- **DBSCAN / HDBSCAN** – for non-spherical clusters and noise handling
- **Gaussian Mixture Model** – probabilistic soft clustering

### Evaluation Metric:
- **Silhouette Score**: Used to evaluate cohesion/separation of clusters

##  Product Recommendation Engine
Based on the clustering output:
- Younger users with high balances → Recommend long-term investments
- Older customers with stable income → Suggest retirement plans
- Low activity users → Recommend savings or credit cards

##  Results
- Cluster analysis revealed 3–5 meaningful customer segments
- Recommendation logic applied per cluster for personalization
- Enhanced customer insights for business decision-making
