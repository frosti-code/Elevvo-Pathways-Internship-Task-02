🛍️ Customer Segmentation using K-Means Clustering

This project applies K-Means clustering to segment mall customers based on their annual income and spending score.

📌 Objective

- Use the Mall Customer Segmentation dataset.
- Group customers into meaningful clusters using unsupervised learning.
- Identify customer types (e.g., high spenders, low income, etc.) to assist with business strategy.

📊 Dataset Overview

The dataset includes the following columns:

- `CustomerID`
- `Genre`
- `Age`
- `Annual Income (k$)`
- `Spending Score (1–100)`

➡️ For this task, we focus on:
- Input Features: `Annual Income (k$)`, `Spending Score (1–100)`
- Goal: Cluster customers without any labels (unsupervised learning)

🧰 Tools & Libraries

- Python 
- pandas
- matplotlib
- scikit-learn

🔍 Steps Performed

1. Data Loading: Imported CSV using pandas.
2. Feature Selection: Used only `Annual Income` and `Spending Score`.
3. Feature Scaling: Standardized features using `StandardScaler`.
4. Elbow Method: Found optimal number of clusters by plotting inertia vs k.
5. K-Means Clustering:
   - Applied KMeans with optimal `k` (usually 5).
   - Assigned cluster labels to each customer.
6. Visualization: Plotted 2D clusters using color-coded scatter plot.
7. Interpretation: Each cluster represents a distinct customer segment.

📈 Results

Model grouped customers into distinct clusters such as:
- 🟢 Low income, low spending
- 🔵 High income, high spending (ideal targets)
- 🔴 High income, low spending (need incentives)
- 🟡 Low income, high spending (risk takers)
- ⚪️ Average customers

Each cluster was visualized clearly using 2D scatter plots with centroids.

🧠 Key Takeaways

- K-Means helps uncover hidden patterns in customer behavior.
- Elbow Method is essential for choosing the right number of clusters.
- Clustering can help personalize marketing and optimize resource allocation.

✅ Future Improvements

- Include `Age` or `Gender` for 3D clustering or deeper analysis.
- Use PCA or t-SNE for dimensionality reduction before clustering.
- Test with DBSCAN or Hierarchical Clustering for non-spherical data.

👨‍💻 Author

Muhammad Mustaqeem Javed — AI/ML Intern  
