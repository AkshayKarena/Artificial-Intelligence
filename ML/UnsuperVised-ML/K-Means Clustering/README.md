# K-Means CLustering Project
## Project Overview
This project applies **K-Means-Clustering** to Analyze petterns in a dataset using Unsupervised Machine Learning.

The Objective was to:-
  - Explore Hidden group Structures in the dataset
  - Determine the optimal number of clusters
  - Compare clustering results using different evalution techniques
  - Visualize clusters using PCA

## Dataset Descripition
The dataset contains multiple numerical features representing characteristics of the data points.
Before applying clustering:
  - Non-numeric columns were removed
  - Selected relevant numerical features
  - Data was standardized using **StandardScaler**


## Project Workflow

### 1️ Data Preprocessing
  - Selected numeric features
  - Removed unnecessary columns
  - Applied feature scaling using:
  \[
  Z = (X - \mu) / \sigma
  \]
(Standardization ensures all features contribute equally.)


### 2️ Initial Clustering (Random K)
  - Applied K-Means with a random choice of K (e.g., K=3)
  - Visualized clusters
  - Observed overlapping regions


### 3️ Elbow Method (WCSS)
To determine optimal number of clusters:
  \[
  WCSS = \sum (distance\ from\ centroid)^2
  \]
  - Computed WCSS for K = 1 to 10
  - Plotted Elbow Curve
  - Observed smooth decline (no sharp bend)
  - Selected K = 6 from elbow approximation


### 4️ Silhouette Score Analysis
Silhouette Score measures:
  - Cluster compactness
  - Cluster separation
  \[
  Score = \frac{b - a}{max(a, b)}
  \]

Where:
  - a = intra-cluster distance
  - b = nearest cluster distance
Result:
  - Highest silhouette score at **K = 2**
  - Overall silhouette values were low (~0.15)
  - Indicates weak cluster separation


### 5️ PCA Visualization
Since high-dimensional data cannot be visualized directly:
  - Applied **Principal Component Analysis (PCA)**
  - Reduced dimensions to 2
  - Plotted clusters in 2D space

Observation:
  - Clusters showed overlapping regions
  - No strong circular separation
  - Indicates dataset is not strongly clusterable

##  Final Analysis
Method              Suggested K        Observation
Random K              3                Overlapping Clusters
Elbow Method          6                Smooth Curve, Weak Elbow
Silhouette            2                Best Separation but low Score


###  Key Insight
  - Dataset does not have strongly distinct cluster boundaries.
  - K-Means forces clusters even when structure is weak.
  - Silhouette score confirmed low cluster separation.


## 🛠️ Technologies Used
  - Python
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - Scikit-learn

