# CryptoClustering

### The project is called "CryptoClustering" and its goal is to predict if cryptocurrencies are affected by 24-hour or 7-day price changes using Python and unsupervised learning techniques.

## The project tasks are as follows:

### 1. Data Preparation:
   - Load the crypto_market_data.csv file into a DataFrame.
   - Perform summary statistics and plot the data to understand its structure.
   - Normalize the data using the StandardScaler() module from scikit-learn.
   - Create a new DataFrame with the scaled data, setting the "coin_id" as the index.

### 2. Find the Best Value for k Using the Original Scaled DataFrame:
   - Use the elbow method to find the optimal value for k (number of clusters).
   - Create a line chart to visualize the inertia values for different values of k.
   - Answer the question: What is the best value for k?

### 3. Cluster Cryptocurrencies with K-means Using the Original Scaled Data:
   - Initialize a K-means model with the best value for k.
   - Fit the model using the original scaled DataFrame.
   - Predict the clusters for the cryptocurrencies and add a new column with the predicted clusters.
   - Create a scatter plot using hvPlot to visualize the clusters.

### 4. Optimize Clusters with Principal Component Analysis (PCA):
   - Perform PCA on the original scaled DataFrame to reduce the features to three principal components.
   - Retrieve the explained variance to determine the information attributed to each principal component.
   - Answer the question: What is the total explained variance of the three principal components?
   - Create a new DataFrame with the PCA data, setting the "coin_id" as the index.

### 5. Find the Best Value for k Using the PCA Data:
   - Use the elbow method on the PCA data to find the optimal value for k.
   - Create a line chart to visualize the inertia values for different values of k.
   - Answer the questions: What is the best value for k when using the PCA data? Does it differ from the best value for k found using the original data?

### 6. Cluster Cryptocurrencies with K-means Using the PCA Data:
   - Initialize a K-means model with the best value for k.
   - Fit the model using the PCA data.
   - Predict the clusters for the cryptocurrencies using the PCA data and add a new column with the predicted clusters.
   - Create a scatter plot using hvPlot to visualize the clusters.

### 7. Visualize and Compare the Results:
   - Create composite plots using hvPlot to compare the elbow curves and the cryptocurrency clusters obtained from the original data and the PCA data.
   - Answer the question: Based on visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data with K-means?

The project has specific requirements for code implementation, data analysis, and visualization. 