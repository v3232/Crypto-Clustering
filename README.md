# Crypto-Clustering

This project applies clustering analysis to cryptocurrency market data using the K-Means algorithm. It demonstrates the effectiveness of dimensionality reduction with Principal Component Analysis (PCA) in improving cluster formation and visualization.

---

## Project Features

1. **Data Preprocessing**:
   - Normalizes the input data using `StandardScaler`.
   - Prepares datasets for clustering with and without PCA transformation.

2. **Clustering**:
   - Implements the K-Means clustering algorithm.
   - Identifies the optimal number of clusters using the Elbow Method.

3. **Dimensionality Reduction**:
   - Reduces data features to three principal components using PCA.
   - Compares clustering results with and without PCA.

4. **Visualization**:
   - Visualizes cluster formations using scatter plots.
   - Displays Elbow Curves to determine optimal clusters.

---

## Key Dependencies

The following Python libraries are required:
- `pandas`: For data manipulation and analysis.
- `hvplot.pandas`: For interactive plotting.
- `scikit-learn`: For machine learning algorithms (K-Means, PCA, StandardScaler).
- `pathlib`: For handling file paths.

## File Structure
.
├── Resources/
│   └── crypto_market_data.csv       # Input CSV file containing cryptocurrency market data
├── crypto_clustering.ipynb          # Jupyter Notebook containing the code
└── README.md                        # Project documentation
└── Scatterplot_without_PCA.png      # png file of the visualisation
└── Scatterplot_with_PCA.png         # png file of the visualisation


## Observations
* Without PCA: The clusters are formed based on all features in the dataset, which might include noise and correlations, leading to less distinct groups.
![Scatterplot_without_PCA](Scatterplot_without_PCA.png)

* With PCA: Dimensionality reduction improves clustering performance, forming more discrete and meaningful clusters.
![Scatterplot_with_PCA](Scatterplot_with_PCA.png)
