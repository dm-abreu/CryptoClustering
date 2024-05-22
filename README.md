# Cryptocurrency Clustering Challenge

## Overview
This challenge involves applying K-means clustering and principal component analysis (PCA) to classify cryptocurrencies based on their price fluctuations over various timeframes.

## Setup
- Create a repository named `CryptoClustering`.
- Clone the repository to your local machine.
- Push changes to GitHub.

## Files
- Module 11 Challenge files.

## Instructions
1. Rename `Crypto_Clustering_starter_code.ipynb` to `Crypto_Clustering.ipynb`.
2. Load `crypto_market_data.csv` into a DataFrame and set the index to the `coin_id` column.
3. Obtain summary statistics of the data.

### Data Preparation
- Normalize the data using `StandardScaler()`.
- Create a DataFrame with the scaled data, using `coin_id` as the index.

### K-Means Clustering
- Determine the best value for k using the elbow method.
- Cluster cryptocurrencies using K-Means with the original scaled data.
- Add a new column with the predicted clusters to the original data.
- Create a scatterplot with "price_change_percentage_24h" vs "price_change_percentage_7d".

### Principal Component Analysis (PCA)
- Perform PCA on the original scaled data to reduce features to three principal components.
- Determine the total explained variance of the three principal components.
- Create a new DataFrame with the PCA data, using `coin_id` as the index.

### K-Means Clustering with PCA Data
- Find the best value for k using the elbow method on the PCA data.
- Cluster cryptocurrencies using K-Means with the PCA data.
- Add a new column with the predicted clusters to the PCA data.
- Create a scatterplot with "PC1" vs "PC2".

### Feature Weights Analysis
- Create a DataFrame showing the weights of each feature for each principal component.

## Requirements
- **Best Value for k (Original Data)**: Implement the elbow method to find the best k value.
- **K-Means Clustering (Original Data)**: Initialize K-means with the best k value and fit the model.
- **PCA Optimization**: Create a PCA model instance and reduce features to three principal components.
- **Best Value for k (PCA Data)**: Use the elbow method with PCA data to find the best k value.
- **K-Means Clustering (PCA Data)**: Initialize K-means with the best k value and fit the model using PCA data.
- **Feature Weights Analysis**: Analyze which features have the strongest influence on each component.

### Coding Conventions and Formatting
- Place imports at the top of the file.
- Use lowercase characters for functions and variables, separated by underscores.
- Follow DRY principles and use concise logic.

### Deployment and Submission
- Submit a link to the GitHub repository containing your files.
- Use the command line for adding files to the repository.
- Include appropriate commit messages.

### Code Comments
- Ensure the code is well-commented for understanding by other developers.
