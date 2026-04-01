Mini Project: Evaluating Clustering Before and After PCA
Objective

The aim of this project is to investigate the effect of dimensionality reduction on clustering performance. Specifically, it evaluates how Principal Component Analysis (PCA) influences clustering results and visualization clarity. The study compares clustering outcomes before and after applying PCA on a dataset with multiple numerical features.

Dataset
Recommended: Wine Dataset from sklearn.datasets.load_wine
Type: Numerical, multi-feature dataset suitable for clustering
Custom datasets with multiple numerical features are also acceptable
Methodology
1. Data Preprocessing
Check for and handle missing values
Apply Standardization to scale features using StandardScaler
Ensures all features contribute equally to clustering
2. Clustering Before PCA
Apply K-Means Clustering on the original dataset
Record:
Inertia (within-cluster sum of squares)
Cluster distribution
3. Dimensionality Reduction
Apply PCA to reduce data to 2 principal components
Enables better visualization and removes potential noise
4. Clustering After PCA
Apply K-Means on the PCA-transformed data
Record cluster properties and evaluate performance
5. Visualization
Plot 2D scatter plots using PCA components
Compare clusters before and after PCA visually
6. Analysis
Evaluate impact of PCA on clustering performance:
Did PCA improve cluster separation or clarity?
Was any significant information lost?
Which approach is preferable depending on objectives (accuracy vs visualization)?
Deliverables
Jupyter Notebook (.ipynb) containing:
All code for preprocessing, clustering, PCA, and visualization
Clear and concise explanations of each step
Comparative analysis and key insights
Optional Extensions
Test different numbers of PCA components to evaluate impact on clustering
Compare results with alternative clustering algorithms, such as DBSCAN
Key Insights (Guidelines for Notebook)
PCA often enhances visual interpretability but may lose some feature-specific information
K-Means clustering may produce slightly different results before and after PCA
Optimal approach depends on goal:
Visualization clarity → PCA
Maximal information retention → Original features
