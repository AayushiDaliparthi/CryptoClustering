# Task: CryptoClustering - Predicting Cryptocurrency Price Changes

Objective: Utilize Python and unsupervised learning to predict if cryptocurrencies are influenced by 24-hour or 7-day price alterations.

**Steps**:

```python
Data Preparation:

```
Load the dataset, "crypto_market_data.csv", into a DataFrame.
Obtain summary statistics and visualize the data.
Normalize the data using StandardScaler() from scikit-learn.
Create a new DataFrame with the scaled data, with "coin_id" set as the index.

```python
Determining Optimal k-value:

```
Employ the elbow method to find the best k-value.
Create a range of k-values from 1 to 11.
Compute inertia for each k-value and plot the results.
Answer: What is the optimal k-value?

```python
Clustering with K-means on Original Scaled Data:

```
Initialize K-means model with the optimal k-value.
Fit the model to the original scaled DataFrame.
Predict clusters and append them to the original data.
Visualize clusters using a scatter plot, coloring points based on K-means labels.

```python
Optimizing Clusters with Principal Component Analysis (PCA):

```
Perform PCA on the original scaled DataFrame, reducing features to three principal components.
Determine the explained variance of each principal component.
Create a new DataFrame with PCA data, using "coin_id" as the index.

```python
Finding Optimal k-value Using PCA Data:

```
Apply the elbow method on PCA data to find the best k-value.
Plot inertia values for different k-values.
Answer: What is the best k-value using PCA data? Does it differ from the original data?

```python
Clustering with K-means on PCA Data:

```
Initialize K-means model with the optimal k-value obtained from PCA.
Fit the model to the PCA data.
Predict clusters and add them to the PCA DataFrame.
Visualize clusters using a scatter plot, coloring points based on K-means labels.

```python
Analyzing Impact:

```
Reflect on the impact of using fewer features for clustering with K-Means.
