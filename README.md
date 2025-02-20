# Clustering Airplane Passenger Satisfaction Dataset

##   Overview
This project applies **unsupervised learning techniques**, specifically **K-Means clustering**, to explore the structure of the **Airplane Passenger Satisfaction** dataset. The goal is to group similar passengers based on their features and analyze how well these clusters align with the actual satisfaction labels. **Principal Component Analysis (PCA)** is used for dimensionality reduction to visualize clusters effectively.

##  Features
- **K-Means Clustering**: Groups passengers based on feature similarity.
- **PCA for Dimensionality Reduction**: Reduces feature space to improve clustering and visualization.
- **Evaluation Metrics**: Uses **Silhouette Score, Adjusted Rand Index (ARI), Adjusted Mutual Information (AMI), and V-Measure** to assess clustering quality.
- **Data Visualization**: Displays clusters in **2D and 3D scatter plots**.

##  Dataset
The dataset used in this project is the **Airline Passenger Satisfaction Dataset**, sourced from Kaggle.

 [Airline Passenger Satisfaction Dataset on Kaggle](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)
## Methodology
### **1. Data Preprocessing**
- Removed non-informative **ID columns**.
- Encoded categorical variables using **One-Hot Encoding**.
- Standardized numerical features using **StandardScaler**.
- Applied **PCA** to reduce dimensions for better visualization.

### **2. Clustering Algorithm**
- **K-Means Clustering** with `k=2`.
- Used **sklearn.cluster.KMeans** for implementation.

### **3. Evaluation Metrics**
| Metric | Description |
|--------|------------|
| **Silhouette Score** | Measures how well clusters are separated. |
| **Adjusted Rand Index (ARI)** | Compares predicted clusters with true labels. |
| **Adjusted Mutual Information (AMI)** | Evaluates clustering quality while accounting for randomness. |
| **V-Measure** | Balances **homogeneity** and **completeness** for clustering performance. |

## Results & Discussion
- **For the Airplane Passenger Satisfaction dataset**, K-Means clustering achieved moderate alignment with true labels, though significant overlap was observed between classes.
- **Dimensionality Reduction (PCA)** did not significantly improve clustering performance but helped in visualization.
- **2D & 3D Visualizations** showed that data points were highly overlapped, confirming that K-Means may not be the best approach for this problem.
