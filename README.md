# Clustering and Classification of Music Moods Using Spotify Audio Features

## Project Overview
This project applies data mining and machine learning techniques to discover and predict music moods using Spotify audio features.

The project follows a **two-phase approach**:
1. **Unsupervised Learning (Clustering)**
2. **Supervised Learning (Classification)**

The goal is to first identify natural groupings in music data, then use those groupings as labels for predictive modeling.

---

## Dataset
- **Spotify Audio Features Dataset (April 2019)**
- ~130,000 tracks
- 17 audio-related attributes (energy, valence, danceability, etc.)
- No predefined labels (unsupervised setting)

---

## Phase 1: Clustering
### Models Used
- **K-Means Clustering**
- **Gaussian Mixture Model (GMM)**

### Feature Selection
Selected features based on correlation analysis:
- energy
- valence
- danceability
- acousticness
- instrumentalness
- speechiness

### Evaluation Metrics
- Silhouette Score
- Davies–Bouldin Index
- PCA visualization

### Result
K-Means achieved better cluster separation and lower Davies–Bouldin score compared to GMM and was selected as the final clustering method.

Clusters were interpreted as:
- Party Mood
- Night Drive
- Acoustic Soul

---

## Phase 2: Classification
After generating mood labels from clustering, the task was converted into a supervised classification problem.

### Models Used
- **Random Forest Classifier**
- **K-Nearest Neighbors (KNN)**

### Evaluation
- Random Forest achieved **perfect accuracy (1.00)** in reproducing cluster labels
- KNN achieved ~97% accuracy
- Confusion matrices and feature importance were analyzed

> Note: Classification accuracy reflects how well models reproduce cluster labels, not true ground-truth mood accuracy.

---

## Visualization
- Correlation heatmaps
- PCA cluster visualization
- Mood distribution plots
- Feature importance analysis
- Confusion matrices

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn, Plotly
- Google Colab

---

## Key Takeaways
- Audio features can effectively capture music mood patterns
- K-Means provided clear and interpretable clusters
- Random Forest demonstrated strong separability of mood-based clusters

---

## Author
Rama Abdoh



