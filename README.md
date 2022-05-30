# Cryptocurrencies
Challenge 18: Crypotocurrencies Data Analysis Using Unsupervised Machine Learning Techniques

## Project Overview
The purpose of this project it to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. Since there is no known output for what we are looking for, we have decided to use unsupervised learning. 
 
 ## Resources
Data Source: crypto_data.csv
- Python 3.9.0
- Anaconda Navigator 2.1.1, Jupyter Notebook 6.4.6,

## Results
#### Deliverable 1: Preprocessing the Data for PCA
The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. 

#### Deliverable 2: Reducing Data Dimensions Using PCA
The Principal Component Analysis (PCA) algorithm was applied to reduce the dimensions of the data frame to three principal components.

#### Deliverable 3: Clustering Cryptocurrencies Using K-means
- Clustering is a type of unsupervised learning that groups data points together.
- K-means is an unsupervised learning algorithm used to identify and solve clustering issues.
- The K-means algorithm is used to cluster the cryptocurrencies using the PCA data, where the following steps have been completed:
  - An elbow curve is created to find the best value for *K* (*K*-> number of clusters)
  <img src="/Resources/img1.png" width="50%" height="50%">
  
  - Predictions are made on the K clusters of the cryptocurrencies’ data and another column is added to the clustered_df named Class that holds the predictions
   <img src="/Resources/img2.png" width="50%" height="50%">


#### Deliverable 4: Visualizing Cryptocurrencies Results
- The clusters are plotted using a 3D scatter plot, and each data point shows the CoinName and Algorithm on hover
<img src="/Resources/img4.png" width="50%" height="50%">

- A table with tradable cryptocurrencies is created 
<img src="/Resources/img5.png" width="50%" height="50%">

- The total number of tradable cryptocurrencies is printed: *There are 532 tradable cryptocurrencies*.

- A DataFrame is created that contains the *clustered_df* DataFrame index, the scaled data, and the CoinName and Class columns 
<img src="/Resources/img3.png" width="50%" height="50%">

- A *hvplot scatter plot* is created where the X-axis is *"TotalCoinsMined"*, the Y-axis is *"TotalCoinSupply"*, the data is ordered by *"Class"*, and it shows the CoinName when you hover over the data point 
<img src="/Resources/img7.png" width="50%" height="50%">

