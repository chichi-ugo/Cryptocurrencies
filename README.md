# Cryptocurrencies
Cryptocurrency Data exploration using Unsupervised Machine Learning

## Purpose
In this analysis, we aimed to analyze cryptocurrency data and use unsupervised machine learning models to uncover trends in the data that may influences investors.

We preprocessed the data using pandas in order to fit the models, then used clustering algorithms to group the data points and make visualizations.

## Results
After the data is preprocessed - transformed to drop null values, filtering for columns of most interest, numerically encoding the categorical data - the data was then scaled. With the scaled data, we were able to perform a principal component analysis (PCA) in order to reduce the dimensions and generate three columns - from 98 - for principal components for our data.

![PCA Results](https://github.com/chichi-ugo/Cryptocurrencies/blob/main/images/pca.PNG?raw=true)

With this analysis, we were then able to generate an elbow graph. With this graph, we are able to determine a k-value for the number of clusters. This is seen in the graph where the curve is seen to change from a predominantly vertical slope to a predominantly horizontal one.

![Elbow Curve](https://github.com/chichi-ugo/Cryptocurrencies/blob/main/images/elbow_curve.PNG?raw=true)

We were also able to have the model make predictions based off our principal component data. These predictions essentially assign each data point to one group out of *k* clusters. With these predictions, we are able to plot the data and display the clustered groups - we depict the data with a 3-D scatter plot.

![3D Plot](https://github.com/chichi-ugo/Cryptocurrencies/blob/main/images/3D_clusters.png?raw=true)

Lastly, we were able to display the tradable currencies in a table and generate a 2-D scatterplot as another look of the data, using the Minmax Scaler. the results are as follows:

![Tradeable table](https://github.com/chichi-ugo/Cryptocurrencies/blob/main/images/tradeable_table.PNG?raw=true)

![2D Plot](https://github.com/chichi-ugo/Cryptocurrencies/blob/main/images/2D_scatter.PNG?raw=true)


## Summary
This analysis provides a good starting point in exploring cryptocurrency data. The unsupervised machine learning module was successful in grouping the data into clusters, however more work will need to be done to interpret whether or not this provides conclusive results as to trends in the crypto-realm.
