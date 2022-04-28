# Cryptocurrencies

## Purpose

Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So our objective is to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data will need to be processed to fit the machine learning models. Since there is no known output for what we are looking for, we are going to use unsupervised learning. To group the cryptocurrencies, we decided on a clustering algorithm. We will use data visualizations to share our findings.

## Results

In order to use unsupervised learning, we preprocessed and transformed the data accordingly. This entails dropping the null values, using tradable and mined cryptocurrencies, numerically encoding categorical columns, and scaling the data.

### **Clustering Cryptocurrencies Using K-Means - Elbow Curve**

In order to visualize how many clusters we can divide the cryptocurrencies into, we created an elbow curve.

![elbow_curve](https://user-images.githubusercontent.com/95505596/165859904-54fd467f-74df-423f-b84a-13e20718f8a1.png)

### **Visualizing Cryptocurrencies Results - 3D-Scatter with Clusters**

We created a 3D scatter plot that located each clustered cryptocurrency in relation to the 3 principal components created on the PCA.

![scatter](https://user-images.githubusercontent.com/95505596/165860098-bddd5013-40a6-4eaf-9cf8-3ccd5c167fd5.png)

### **Tradable Cryptocurrencies Table**

![tradable_crypto](https://user-images.githubusercontent.com/95505596/165860266-167bdbcf-f627-4420-9d91-7e813ae773ab.png)

### **2D-Scatter plot (TotalCoinMined vs TotalCoinSupply)**

Graphing the clustered cryptocurrencies by total coins mined and the total coin supply we can clearly see two outliers.

![hvplot](https://user-images.githubusercontent.com/95505596/165860292-b2317b73-df50-42f8-93c4-95728cb3c1ca.png)

## Summary

We have demonstrated that cryptocurrencies can be clustered with the help of unsupervised machine learning. Identifying the classification of 532 cryptocurrencies helped us find clustering patterns and find underlying outliers. We have just scratched the surface. With some further research we can determine the potential of these cryptocurrencies and possible new ones.
