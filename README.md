oline Stores – Customer Segmentation & Insights

This project analyzes customer purchasing behavior from an online retail dataset and applies unsupervised learning techniques to segment customers. It provides actionable insights to support personalized marketing, fraud detection, and business planning.

##  Project Objective

- Derive insights from customer purchase history.
- Segment customers using K-Means clustering.
- Visualize and interpret customer groups for business use.

##  Data Preprocessing

- Handled special characters using `unicode_escape`.
- Removed records with missing `CustomerID`.
- Converted `InvoiceDate` to datetime format.
- Created `TotalAmount = Quantity × UnitPrice`.

## Feature Engineering

- Aggregated metrics at the customer level:
  - **NumPurchases**: Unique invoices
  - **TotalQuantity**: Total units bought
  - **TotalSpend**: Total monetary spend
  - **AvgUnitPrice**: Mean price per item

##  Feature Scaling & Clustering

- Standardized features using `StandardScaler`.
- Chose optimal clusters (`k=4`) using the Elbow Method.
- Applied **KMeans** clustering and labeled each customer.

##  Visualization & PCA

- Used PCA to reduce dimensionality and visualize clusters in 2D.
- Plotted PCA1 vs PCA2 to observe separation between customer types.

##  Cluster Interpretation

| Cluster | Segment Name          | Characteristics                                        |
|--------|------------------------|---------------------------------------------------------|
| 0      | Average Shoppers       | Medium spend and frequency                             |
| 1      | High-Value Customers   | Frequent buyers with high spend                        |
| 2      | Regular Customers      | Consistent, balanced buyers                            |
| 3      | Refund-Prone Customers | Negative spend, low quantity, high price (possible fraud) |

##  Additional Insights

- Sales peaked during holidays.
- Refund behavior identified through negative `TotalSpend`.
- Segment distribution shown in bar charts.

##  Business Value

- Enables **targeted marketing** and **loyalty programs**.
- Identifies **refund-prone customers** for fraud control.
- Supports **operational planning** with sales trends.

## Tools & Libraries

- **Python**, **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn** for visualizations
- **Scikit-learn**: `KMeans`, `PCA`, `StandardScaler`

##  File

- `Shylaja_onlineretail_project.ipynb`: Main notebook with code and insights.

##  Conclusion

This project combines exploratory data analysis, feature engineering, feature scaling unsupervised learning, and business interpretation to uncover meaningful customer patterns that support better decision-making.


