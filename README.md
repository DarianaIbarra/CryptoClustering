**Determine the Optimal k Value Using the Elbow Method on the Original Scaled Data
Follow these steps to identify the best number of clusters (k):**

-Generate a list of k values ranging from 1 to 11.

-Create an empty list to store the inertia values for each k.

-Use a loop to compute the inertia for each k value.

-Organize the collected data into a dictionary for visualization.

-Plot an elbow curve to observe how inertia changes with different k values and determine the optimal k visually.

-Answer this question in your notebook: What is the best k value?

**Cluster Cryptocurrencies Using K-Means on the Original Scaled Data
Use the following steps to group cryptocurrencies based on the best k value:**

-Initialize a K-Means model with the optimal k value.

-Train the model on the original scaled dataset.

-Predict the cluster assignments for each cryptocurrency.

-Create a copy of the dataset and add a new column to store the predicted cluster labels.

-Visualize the clustering with a scatter plot using hvPlot:

-Set "price_change_percentage_24h" as the x-axis and "price_change_percentage_7d" as the y-axis.

-Color the data points based on their assigned clusters.

-Enable hover functionality to display the coin_id of each cryptocurrency.

**Optimize Clustering with Principal Component Analysis (PCA)
Using the original scaled dataset, apply PCA to reduce dimensionality:**

-Perform PCA and reduce the dataset to three principal components.

-Retrieve the explained variance of each component to understand the distribution of information.

-Answer this question in your notebook: What is the total explained variance of the three principal components?

-Create a new DataFrame containing the PCA-transformed data, setting "coin_id" as its index.

-Display the first five rows of the PCA-transformed DataFrame.

**Determine the Best k Value Using the PCA Data
Apply the elbow method to the PCA data to find the optimal k:**

-Create a list of k values from 1 to 11.

-Generate an empty list to store inertia values for each k.

-Use a loop to compute inertia for each k value.

-Store the computed values in a dictionary for visualization.

-Plot an elbow curve to determine the most suitable k value.

-Answer these questions in your notebook:

-What is the best k value when using PCA data?

-How does it compare to the k value found with the original data?

**Cluster Cryptocurrencies Using K-Means on the PCA Data
Follow these steps to apply K-Means clustering to the PCA-transformed data:**

-Initialize a K-Means model using the best k value.

-Train the model on the PCA data.

-Predict the cluster assignments for the cryptocurrencies.

-Create a copy of the PCA DataFrame and add a column to store the cluster labels.

-Visualize the clustering with a scatter plot using hvPlot:

-Set "price_change_percentage_24h" as the x-axis and "price_change_percentage_7d" as the y-axis.

-Color the data points based on the assigned clusters.

-Include the coin_id in the hover settings for easy identification.

-Reflect on this question: How does reducing the number of features impact clustering using K-Means?

