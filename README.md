# E-Commerce Transactions Dataset Analysis
Given `Customers.csv`, `Products.csv`, `Transactions.csv` forming a eCommerce Transactions dataset to be used for performing EDA, extracting insights, developing predictive models and performing customer segmentation.

## Task 1
- It can be observed that none of the 3 csv's have null values and outliers. 
- Business Insights Extracted:
  - The platform is most famous in the **South American continent** compared to other continents when total active customers are compared.
  - The platform is becoming more and more popular among **North American** customers as it has the highest number of people who have signed up in the past 1 year.
  - It is observed that **ActiveWear SmartWatch** is the most popular item among customers on the platform.
  - New customers in **Asia and Europe** tend to spend more on an average compared to old customers of the same continent which is exactly the opposite in **North and South America.**
  - **Home Decor** products are priced less on an average and people have bought them the least among other product categories, it may be because people are not satisfied with quality of these products.
  - Products in the **Books** category are priced higher on an average compared to other categories and it is the most popular category of items people shop for.
  - People make the most purchases during December-January **(New Year period)** and July-September **(Fall period)**.

## Task 2
- For calculating similarity score of each pair of customers out of 5, **both personal and product info is used:**
  - **Region:**  
    - Increment total score by 1 if both customers belong to same region
  - **Signup Date:**
    - Increment total score by 1 if both customers are classified as same (if both are Old or both are New)
  - **Average TotalValue spent:**
    - For calculating similarity score purposes, the difference between the TotalValue is considered and finally increment ranges from [0,1].
  - **Top 2 Product Categories for the customer:**
    - Increment total score by 2, if both the top categories match.
    - Increment total score by 1, if any one of the top categories match.

## Task 3
- Applied **K-Means** clustering algorithm.
- Visualized clusters after dimensionality reduction using **PCA and t-SNE**.
- Number of clusters: 4
- DB Index: 1.36
- Silhouette Score: 0.24

