# K-Means Clustering (Mall Customers Dataset)

## 📘 Project Overview
This project demonstrates **Unsupervised Learning** using the **K-Means Clustering** algorithm.  
The goal is to group mall customers based on their **age, income, and spending score** to identify customer segments.  
By using visualization and evaluation metrics, we find meaningful clusters that describe customer behavior.

---

## 🧰 Tools & Libraries Used
- **Python**
- **Pandas** – data handling
- **NumPy** – numerical operations
- **Matplotlib / Seaborn** – data visualization
- **Scikit-learn** – model building, scaling, and evaluation

---

## 🧩 Steps Performed

### 1️⃣ Load & Explore Dataset
- Imported the `Mall_Customers.csv` dataset.
- Checked for null values and data types.
- Dropped unnecessary columns (`CustomerID`).

### 2️⃣ Preprocessing
- Encoded the **Gender** column (Male → 0, Female → 1).  
- Standardized the numerical features for better cluster separation.

### 3️⃣ Elbow Method
- Used **Inertia (Within-Cluster Sum of Squares)** to find the optimal number of clusters.
- Plotted K (1–10) vs Inertia curve.
- Found **K = 5** as the best choice for this dataset.

### 4️⃣ Model Training
- Trained **KMeans** with 5 clusters.
- Assigned each customer a **cluster label**.

### 5️⃣ Visualization
- Applied **PCA** to reduce data into 2D for easy visualization.
- Plotted colorful scatter plots to display clusters.

### 6️⃣ Evaluation
- Calculated **Silhouette Score** to measure how well-defined the clusters are.
- Higher silhouette value → better clustering performance.

### 7️⃣ Cluster Analysis
- Computed average values of **Age**, **Income**, and **Spending Score** per cluster.
- Interpreted clusters as different customer groups (e.g., high income–low spending, etc.).

---

## 📊 Visualization Samples
| Visualization | Purpose |
|----------------|----------|
| `plt.plot(range(1,11), inertia_scores)` | Find the optimal number of clusters |
| `sns.scatterplot(x='PCA1', y='PCA2', hue='Cluster')` | Visualize cluster distribution |
| `sns.heatmap(cluster_summary)` | View feature averages across clusters |

---

## ✅ Results
- Optimal clusters found: **5**  
- Achieved a good **Silhouette Score**, indicating clear customer segmentation.  
- Discovered patterns like:
  - 🧍‍♂️ **Cluster 1:** High income – high spending  
  - 🧍‍♀️ **Cluster 2:** Low income – low spending  
  - 🧠 Useful insights for targeted marketing.

---

## 💾 Files Included
- `Mall_Customers.csv` — Original dataset  
- `KMeans_Clustering.ipynb` — Full code  
- `README.md` — Project documentation  

---

## 📚 Learning Outcome
Through this project, I learned:
- How **K-Means clustering** groups similar data points.  
- How to use the **Elbow Method** to choose the best K.  
- How to interpret **Silhouette Score** and visualize clusters in 2D.

---

## 🧑‍💻 Author
**Ganesh R**  
*(Junior AIML Engineer Trainee)*
