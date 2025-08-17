# Mall Customer Segmentation

## Project Overview
This project applies **unsupervised learning techniques**, specifically **Clustering** and **Dimensionality Reduction**, to identify patterns in mall customer behavior. The goal is to segment customers based on demographics and spending habits for better insights.

## Dataset
- **File:** `Mall_Customers.csv`  
- **Rows:** 200  
- **Columns:** `CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`  

## Objective
- Segment customers into meaningful groups  
- Apply **PCA** for dimensionality reduction  
- Use **K-Means Clustering** to identify distinct customer segments  

## Data Preprocessing
- Checked for missing values → None found  
- Checked for duplicates → 0 duplicates  
- Encoded `Gender` column (Male → 0, Female → 1)  
- Scaled features using `StandardScaler`  
- Dropped `CustomerID` as it is irrelevant to clustering  

## Dimensionality Reduction (PCA)
- PCA applied with 2 components for visualization  
- Explained variance:  
  - Component 1: 33.7%  
  - Component 2: 26.2%  

## Clustering (K-Means)
- **Elbow Method** used to determine optimal clusters → k = 5  
- KMeans applied to group customers into 5 segments  

## Clustering Evaluation
- **Silhouette Score:** 0.272 (low but acceptable)  
- **Davies-Bouldin Index:** 1.181 (moderately good)  
- Interpretation: Clusters are distinguishable with slight overlap  

## Conclusion
- PCA helped reduce dimensionality for visualization  
- KMeans successfully segmented customers based on age, income, and spending behavior  
- Evaluation metrics indicate the clusters are valid  

## Files in Repository
- `Mall_Customers.csv` → dataset  
- `mall_segmentation.ipynb` → notebook containing all preprocessing, PCA, KMeans, and visualizations  

## How to Run
1. Clone the repository  
2. Install required libraries:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
3. Open `mall_segmentation.ipynb` and run all cells

## Contact Me

Connect with me on LinkedIn: [Muhammad Hassaan Munir](https://www.linkedin.com/in/muhammad-hassaan-munir-79b5b2327/)
