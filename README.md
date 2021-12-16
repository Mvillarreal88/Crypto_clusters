# Crypto_clusters unsupervised learning

### Analysis:

The goal of this investment portfolio is to provide the client with a classification system for their new investments using machine learning. We will be using crypto data to make this determination and produce models.

### Data Prep:

• The first step is to load the csv and create a DF where we can visualize what the raw data looks like.
• When this is completed we start by removing all crypto that is not currently being traded, as this is data we are not interested in.
• Filtering the crypto that is actually mined is the next step in this process and removing all coins that have a value of 0.
• I order for our dataset to be compatible with machine learning we need the data to be numeric, so we use get_dummies on the columns that are not numeric.

### Dimensionality reduction:

• We have already increased the number of features in the dataset so we now want to perform dimensionality reduction with PCA. we are trying to preserve 90% of the explained variance in this reduction. 
• Next, we further want to reduce the dimensions using t-SNE and create a scatter plot of the output. 

![Screenshot 2021-12-15 183303](https://user-images.githubusercontent.com/81705144/146286360-096ca2eb-eaa0-4bde-be03-611721ba24e3.png)


### K-means:
• Finally we create an elbow plot to identify the best number of clusters. 

![Screenshot 2021-12-15 183303](https://user-images.githubusercontent.com/81705144/146286329-762147f1-5979-47e8-aedc-b29e20ecc691.png)


### Final thoughts:

- Based on the elbow curve it is difficult to make recommendations based on the clusters. This is a continual regression with no curve that we can make a recommendation on.

>- Matthew Villarreal
