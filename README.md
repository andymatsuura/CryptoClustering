# CryptoClustering

## Module 19 Challenge

In this Challenge, we used python and the module SKLearn to utilize unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes. We use the elbow method to find the optimal amount of clusters, then plot the results with KMeans. Then, using principal component analysis, the effects of reductions in dimensionality are visualized. 

First, the original data was scaled and the elbow method was used to find the best value for k. 
![image](https://github.com/andymatsuura/CryptoClustering/assets/150174589/6d15cf21-6ff7-4b9d-b2a0-e606b110b127)

From this graph, the best value for k appears to be 4. A scatter plot based on 4 clusters is as follows.
![image](https://github.com/andymatsuura/CryptoClustering/assets/150174589/027a8d30-1a3b-44f2-a9e0-8972dd826936)
There are 2 clusters with only 1 value each, and clusters are not easy to differentiate. 

We then used the PCA function from sklearn to reduce the dimensionality of the data into 3 components. 

The elbow curve with the PCA data was very different to the original scaled data. 
![image](https://github.com/andymatsuura/CryptoClustering/assets/150174589/41274f45-0cef-4393-aa34-fdd2f038a971)
This elbow graph shows the optimal clusters to be 2.

This is the cluster data from the PCA data. 
![image](https://github.com/andymatsuura/CryptoClustering/assets/150174589/2ceda675-fbce-4dc7-ae00-17d8f04e4f2f)
The clusters look more precise and there are fewer cluster groups

## Conclusion

Through this challenge, we were able to see the difference between using original and modified PCA data and their effects on clustering. It seems to explain more of the variance, and groups the clusters more accurately
