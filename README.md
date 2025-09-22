Hello) 
Wine Data Science Project - Analysis Overview

This project demonstrates a comprehensive analysis of wine quality data, combining regression modeling, feature importance evaluation, clustering, dimensionality reduction, anomaly detection, and data visualization.

1. **Data Preparation**
   - Red and white wine datasets were loaded from CSV files and combined.
   - A binary feature 'type' was added to distinguish red (0) and white (1) wines.
   - The target variable is 'quality', and all other features are considered predictors.
   - Train-test split was performed (80/20), and scaling (RobustScaler) was applied for regression models.

2. **Regression Modeling**
   - Three models were trained and evaluated: Gradient Boosting Regressor (GBM), Support Vector Regressor (SVR), and Multi-Layer Perceptron (MLP).
   - Hyperparameter tuning was performed using GridSearchCV.
   - R² and MSE metrics were calculated to compare model performance.
   - GBM allows direct feature importance extraction, while permutation importance was used for SVR.

3. **Feature Importance**
   - The importance of each feature was visualized using bar plots.
   - This helps to identify which chemical properties of wine contribute most to its quality.

4. **Clustering Analysis**
   - KMeans clustering was applied after StandardScaler normalization.
   - The elbow method suggested 3 clusters.
   - Visualizations include:
     - Scatterplots of alcohol vs volatile acidity colored by cluster.
     - Heatmaps showing mean values of features per cluster.
     - Boxplots comparing wine quality across clusters.
   - PCA was applied for dimensionality reduction:
     - 2D and 3D interactive scatterplots of clusters were generated using Plotly.
     - Graphs are saved as PNG files in the 'plots' folder.

5. **Anomaly Detection**
   - Isolation Forest was used to detect anomalous wines separately for red and white classes.
   - Comparison tables show how anomalies differ from the class mean for all features.
   - This allows identifying unusual wines that may require further investigation.

6. **Note**
   - The analysis includes interactive visualizations and plots that will only display correctly when the code is executed.
   - For full insight, it is recommended to run the code to explore graphs and results dynamically.

The project demonstrates end-to-end workflow in wine data analysis, combining statistical modeling, machine learning, clustering, PCA visualization, and anomaly detection.
