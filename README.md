# SageMaker Unsupervised Learning

## Project: Population Segmentation

### Source 

Project 2 from Udacity's [Machine Learning Engineer Nanodegree](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009t)

### Description

Performing population segmentation in Amazon SageMaker using unsupervised learning to find natural grouping in population data that reveal feature-level similarities between different regions in the US.

- Loaded data from S3, retrieved IAM role and SageMaker session
- Preprocessed, normalized, and visualized data 
- Convert various data into RecordSet format for model fitting 
- Applied dimensionality reduction via Principal Component Analysis (PCA) to reduce the number of features from 34 to 7 
- Loaded PCA model using MXNet 
- Calculate explained variance for various numbers of principal components 
- Examined makeup of PCA components based on weightings of original features and found the top 7 principal components make up ~80% of the data variance
- Deployed PCA model 
- Defining a K-Means model and chose K = 8 (number of clusters) using the Elbow Method 
- Trained and deployed K-Means model 
- Visualized distribution of data across clusters
- Visualized centroids in component space using a 7x8 heatmap
- Found natural groupings by separating regions by labels collected from K-Means model 

### Data 

The data was collected by the [US Census](https://en.wikipedia.org/wiki/United_States_Census), 
which aims to count the US population, recording demographic traits about labor, age, population, and so on, 
for each county in the US. 
