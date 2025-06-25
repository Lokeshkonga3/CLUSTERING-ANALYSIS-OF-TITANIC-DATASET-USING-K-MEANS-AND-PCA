# CLUSTERING-ANALYSIS-OF-TITANIC-DATASET-USING-K-MEANS-AND-PCA
# 🚢 Titanic Clustering with K-Means & PCA

This project applies **unsupervised machine learning** techniques to cluster passengers from the Titanic dataset using **K-Means** and visualizes the results using **PCA**. It focuses on feature selection, data standardization, clustering, and dimensionality reduction.

---

## 📁 Files Included

- `titanic.csv` – The Titanic dataset
- `titanic_kmeans_clustering.ipynb` – The main notebook/script
- `README.md` – Project documentation

---

## 🎯 Objectives

- Select relevant numeric features for clustering.
- Standardize the dataset for meaningful distance metrics.
- Use **K-Means Clustering** to group passengers.
- Determine the optimal number of clusters using the **Elbow Method**.
- Use **PCA (Principal Component Analysis)** to reduce dimensionality to 2D for visualization.
- Visualize the clusters using **Seaborn** and **Matplotlib**.

---

## 🧹 Data Preprocessing

| Step                         | Action Taken                                 |
|------------------------------|----------------------------------------------|
| Feature Selection            | `Age`, `Fare`, `Pclass`, `SibSp`, `Parch`    |
| Missing Value Handling       | Drop rows with missing values                |
| Standardization              | Applied `StandardScaler` from `sklearn`      |

---

## 🔍 Clustering

### K-Means Algorithm
- Used `sklearn.cluster.KMeans`
- Elbow method to find the optimal `k` (clusters)
- Final model applied with `k = 3` (adjustable)

### PCA
- Used `sklearn.decomposition.PCA`
- Reduced 5D data to 2D for visualization

---

## 📈 Visualizations

1. **Elbow Method Plot** – To determine optimal cluster count.
2. **Cluster Visualization using PCA** – Color-coded passenger clusters on a 2D scatter plot.

---

## 📦 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn` (`KMeans`, `PCA`, `StandardScaler`)

---

## ▶️ How to Run

1. Upload the `titanic.csv` file when prompted in Google Colab or Jupyter.
2. Run the notebook or script to:
   - Clean and scale data
   - Determine clusters with K-Means
   - Visualize using PCA

---

## ✅ Results

- Passengers grouped into clusters based on travel class, age, fare, and family size.
- PCA visualization reveals natural groupings within the dataset without supervision.

---

## 📝 Next Steps

- Analyze cluster composition: average age, fare, etc.
- Try other clustering methods (e.g., DBSCAN, Agglomerative).
- Integrate categorical variables using embedding or encoding.

---

## 🤝 Contributing

Feel free to fork and suggest improvements, or use it in your portfolio.

---

## 📃 License

This project is open-source under the [MIT License](LICENSE).
