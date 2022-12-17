# Customer-Segmentation-using-K-means-Clustering

• Implemented K-means clustering Algorithm on dataset of 350 customer samples to identify the segments. 

• Performed dimensionality reduction using Principal Component Analysis to focus on required metadata. 

• Accomplished segmentation of the dataset with 77.20 percent accuracy

Here are some screenshots of my work:

<img width="563" alt="CS_1" src="https://user-images.githubusercontent.com/68967101/208257253-805a5d58-7a5a-4c96-b2c5-eb4ada5ddb00.png">

* Applied Principal Component Analysis (PCA) to discover which dimensions best maximize the variance of features involved. 

* Then, we have considered three features from the dataset as the useful columns. Customer ID is not a useful feature which has been dropped earlier and It does not appear in the final dataset.

* During the fitting process, the model learns some quantities from the data the "components" and "variance".

* We have represented this using a type of scatter plot called biplot by coding our custom function. Each point is represented by its score regarding the principal components. It is helpful to understand the reduced dimensions of the data. It also helps us discover relationships between the principal components and the original variables.

* In the graph Var1 is the Spending Score,Var2 is the Age and Var3 is the Annual Income. We can observe that Annual Income as well as Spending Score as the two most important components.


<img width="546" alt="cs2" src="https://user-images.githubusercontent.com/68967101/208257277-8618461c-1ee8-409c-a151-a57b41477c6f.png">

* Fixed the numbers of clusters to use.There are several direct methods to perform this, among them, we have used the elbow method.  

* The Elbow method emphasizes on how the total WSS(Within-cluster sum of square) varies with the number of clusters.We have then computed k-means by using the Kmeans function which we have imported from sklearn.cluster, for a range of different values of k. Lastly,  the total WSS is calculated. 

 * The curve WSS vs number of clusters is plotted.Finally,the elbow or bend of the plot is located. This point is considered to be the appropriate number of clusters which is our case '5'.


<img width="380" alt="cs3" src="https://user-images.githubusercontent.com/68967101/208257286-c90fd42d-9f7e-478d-a17f-2d97a0b91311.png">


Visualizing the clusters for k=5

The scatterplot of the clusters and their respective centroids has been plotted and the following inferences can be dervied.

 
 1. The orange color(Cluster 1) represents the customers who have average  
    income and are also average spenders.These customers do not over-spend, 
    whatever the offer might they will not spend high, as such their needs
    are already well catered.    

 2.  The salmon color(Cluster 2) represents the customers who earn more but 
    are highly considerate spenders.These customers are very reserved on
    what they spend as such, a database can be collected about their
    specific interests and notifications about the availability of 
    those products can be sent to these customers. 


 3. The violet color (cluster 3) represents the customers who have low income
    and spend the least.These customers are highly mindful of their spendings 
    and will only spend if there it is necessary.To get the most out from these
    customers a database can be created to record, on what commodities they 
    spend and according to their needs the availability,prices and discounts
    should be offered.


    
 4. The green color (cluster 4) represents the customers who have higher
    income and spend the most.These customers should be targeted positively.
    These customers will provide us high income with their large spendings.
    Special treatment for these customers could be provided to these people.
    Premier membership cards and special access to the products could be
    given so that the customers feel special and remain in a loyal base.



 5. The dodgerblue color (cluster 5) represents the customers who have low 
    income but spend higher or have high spending scores.These are erratic
    spenders who can be targeted very easily.If the availability of the required
    goods is made known to these customers then there are high possibilities
    returns will be higher.
    








 





