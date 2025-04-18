# 📊 Clustering using Scikit-Learn

This project conducts a **comparative analysis** of three clustering algorithms—**KMeans**, **Hierarchical Clustering**, and **Mean Shift**—on the popular **Iris dataset**, under multiple preprocessing scenarios.

## 🔍 Objective

To compare the performance of different clustering algorithms on various versions of preprocessed data using standard clustering evaluation metrics.

---

## 🧠 Algorithms Compared

- **KMeans Clustering**
- **Agglomerative (Hierarchical) Clustering**
- **Mean Shift Clustering**

---

## ⚙️ Preprocessing Techniques Applied

The dataset is transformed using the following approaches before clustering:

1. **No Processing** (Raw data)
2. **Normalization** (MinMaxScaler)
3. **Standardization** (StandardScaler)
4. **PCA** (Principal Component Analysis with 2 components)
5. **Standardization + Normalization** (T+N)
6. **Standardization + Normalization + PCA** (T+N+PCA)

---

## 📈 Evaluation Metrics

Each clustering result is evaluated using:

- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Score**

---

## 📊 Visualizations

The project also includes a **bar plot** to visualize Silhouette Scores for KMeans clustering across different preprocessing pipelines and cluster sizes.

---

## 🗃️ Dataset

- **Name**: Iris Dataset
- **Source**: `sklearn.datasets.load_iris()`
- **Features**: 4 (Sepal Length, Sepal Width, Petal Length, Petal Width)
- **Classes**: 3

---

## 📁 Project Structure

```
├── clustering_comparative_study.py  # Main script
├── clustering_comparison_results.csv  # (Optional) Saved results
└── README.md
```

---

## 🚀 How to Run

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/clustering-comparative-study.git
   cd clustering-comparative-study
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the script**
   ```bash
   python clustering_comparative_study.py
   ```

---

## 📝 Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

*(All can be installed using `pip install -r requirements.txt`)*

---

## 📌 Key Insights

- PCA drastically improves performance on Mean Shift clustering.
- Normalization + PCA gives balanced performance for KMeans.
- Hierarchical clustering is consistent across different preprocessing types.

---


## 📚 License

This project is open-source and available under the [MIT License](LICENSE).
