# Cryptocurrencies
![image](https://user-images.githubusercontent.com/112978144/226145892-3095d3e2-fa83-40f6-8a1c-d5ef248eac90.png)
# overview of the challenge
Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked us to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.
In this challenge we used machine learning using unsupervised algorithms, which help us explore data when we're not sure what we're looking for. We analyzed data without a clear output in mind.
we worked primarily with the K-means algorithm, the main unsupervised algorithm that groups similar data into clusters. We built on this by speeding up the process using principal component analysis (PCA), which employs many different feature.


In this assignment there are four technical analysis parts that we need to submit 

Part 1: Preprocessing the Data for PCA
Part 2: Reducing Data Dimensions Using PCA
Part 3: Clustering Cryptocurrencies Using K-means
Part 4: Visualizing Cryptocurrencies Results

# Part 1- Preprocessing the Data for PCA
After completing all the requirements of processing data we got the following results
![image](https://user-images.githubusercontent.com/112978144/226146325-afae2bd1-c8f2-4a77-9bd3-79c9b624e4f6.png)

# Part 2: Reducing Data Dimensions Using PCA
we got following Data Dimensions using PCA 
![image](https://user-images.githubusercontent.com/112978144/226146471-d1b6eefd-dc1b-48bc-a3f6-72b566b4a397.png)

# Part 3: Clustering Cryptocurrencies Using K-means
we find best value for K using elbow curve
![image](https://user-images.githubusercontent.com/112978144/226146596-6eb47758-9ce5-4d29-8bec-74c74a57848a.png)


## we use K-means to cluster data and got following output
![image](https://user-images.githubusercontent.com/112978144/226146560-2d2fb208-f1b3-41c5-860b-d7e624d5ae0f.png)

# Part 4: Visualizing Cryptocurrencies Results
We created a 3D scatter plot using the Plotly Express scatter_3d() function to plot the three clusters from the clustered_df DataFrame.
![image](https://user-images.githubusercontent.com/112978144/226146640-f090a201-3050-4569-98b3-7aa8109cdd67.png)
* we create a table with tradable cryptocurrencies using the hvplot.table() function.


![image](https://user-images.githubusercontent.com/112978144/226146710-870fdbbc-6b5d-455c-9e90-82c37e52ff74.png)
* Class column is added from the clustered_df DataFrame to the new DataFrame.
![image](https://user-images.githubusercontent.com/112978144/226146822-d4ccc5bc-c73c-4672-9c36-dc564a8f9ded.png)

* hvplot scatter plot is created with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class", and have it show the CoinName when you hover over the the data point.
![image](https://user-images.githubusercontent.com/112978144/226146901-12da779e-7a06-449f-8aa7-218e71cfe362.png)

# Summary
![image](https://user-images.githubusercontent.com/112978144/226147217-ffa86526-36a4-4a21-a086-259e0cee6e3e.png)

The unsupervised learning is used to discover hidden structure or patterns in the data, such as clusters, groups, or associations, that can be used to gain insights and make predictions. Unsupervised learning algorithms are often used for exploratory data analysis, data preprocessing, and feature extraction.
Unsupervised learning is used in a wide range of applications, including natural language processing, image recognition, anomaly detection, and recommendation systems.
So from above data bank can easily visualize the data as we can see this analysis is successful at grouping cryptocurrencies into 4 groups though there is lot more scope to find some more information by clustering data.




