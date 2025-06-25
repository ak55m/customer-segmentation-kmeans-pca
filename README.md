
# 🧠 Customer Segmentation Using K-Means++ and PCA

This project uses synthetic e-commerce customer data to segment users based on:

- **Recency**: How recently a customer purchased
- **Frequency**: How often they purchase
- **Monetary**: How much they spend
- **Tenure**: How long they’ve been a customer

## 🔧 Tools
- Python
- scikit-learn
- matplotlib & seaborn
- PCA (Dimensionality Reduction)
- K-Means++ (Clustering)

## 📈 Output: What the Project Does and Finds

This project segments customers into **4 distinct behavioral groups** using the **K-Means++ clustering algorithm**, guided by the following features:

- **Recency**: How recently the customer made a purchase (lower = more recent)
- **Frequency**: How often the customer purchases (higher = more loyal)
- **Monetary**: How much the customer spends (higher = more valuable)
- **Tenure**: How long they've been a customer (higher = more established)

### 🔍 Process Summary:

1. **Data Simulation**: Generated synthetic data for 5,000 customers, mimicking real-world e-commerce metrics.
2. **Standardization**: Scaled all features to ensure fair clustering.
3. **Dimensionality Reduction with PCA**: Compressed the 4 behavioral metrics into 2 components for easy visualization while retaining structure.
4. **Clustering with K-Means++**:
   - Automatically spread out initial centroids for better performance.
   - Grouped customers into 4 segments based on behavioral similarity.
5. **Evaluation**:
   - Used the **Silhouette Score** to assess cluster quality.
   - Visualized clusters in 2D space with color-coded points and centroid markers.
6. **Cluster Profiling**:
   - Generated a summary table showing average Recency, Frequency, Monetary value, and Tenure for each cluster.
   - Insights from this table can guide **marketing**, **loyalty programs**, or **customer retention strategies**.

### 🧠 Example Output (Interpreted):

| Cluster | Recency ↓ | Frequency ↑ | Monetary ↑ | Tenure ↑ | Description           |
|---------|-----------|-------------|-------------|-----------|------------------------|
| 0       | Low       | High        | High        | High      | **VIP Customers**      |
| 1       | High      | Low         | Low         | Low       | **At-Risk / Newbies**  |
| 2       | Medium    | Medium      | Medium      | Medium    | **Average Shoppers**   |
| 3       | Low       | Medium      | Low         | High      | **Infrequent Loyalists**|

*(↓ = lower is better, ↑ = higher is better)*

## 📁 Files
- `kmeans_customer_segmentation.ipynb` – full notebook
- `README.md` – this file

## 🚀 Try it on Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_LINK_HERE)
