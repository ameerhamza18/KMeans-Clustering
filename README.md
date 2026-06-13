# K-Means Clustering on California Housing Data

A step-by-step walkthrough of K-Means clustering using the California Housing dataset. This notebook covers everything from EDA and preprocessing to cluster evaluation and visualization.

---

## 📌 What This Notebook Covers

1. **Intuition** — When and why to use K-Means
2. **EDA & Preprocessing** — Correlation analysis, missing values, outlier handling via IQR
3. **Feature Engineering** — Creating meaningful ratios to reduce redundancy and outliers
4. **Scaling** — StandardScaler for distance-based algorithms
5. **Choosing K** — Elbow method, KneeLocator, and Silhouette scores
6. **Model Training** — KMeans with `k-means++` initialization
7. **Evaluation & Profiling** — Cluster summaries, centroid visualization, PCA 2D projection
8. **Pitfalls to Avoid** — Common K-Means mistakes explained

---

## 📂 Dataset

This project uses the **California Housing dataset** (`housing.csv`).

You can download it from:
- [Kaggle - California Housing Prices](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

Place the downloaded `housing.csv` file inside the `data/` folder and update the notebook path:

```python
df = pd.read_csv('./data/housing.csv')
```

---

## 🛠️ Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/ameerhamza18/KMeans-Clustering.git
cd KMeans-Clustering
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch the notebook

```bash
jupyter notebook notebook/KMeans.ipynb
```

---

## 📦 Requirements

See `requirements.txt` for the full list of dependencies.

---

## 📊 Key Results

| Method | Optimal K |
|--------|-----------|
| Elbow Method | 3 |
| Silhouette Score | 3 |

---

## 📁 Project Structure

kmeans-clustering/

│

├── notebooks/

│   └── KMeans.ipynb       # Main notebook

│

├── data/

│   └── housing.csv        # Dataset (download separately)

│

├── images/                # Saved plots (optional)

│

├── README.md

├── requirements.txt

└── .gitignore

---

## 🧠 Concepts Used

- Unsupervised Learning
- K-Means Clustering
- Elbow Method & KneeLocator
- Silhouette Score
- Principal Component Analysis (PCA)
- IQR-based Outlier Handling
- Feature Engineering

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
