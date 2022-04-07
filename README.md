## **Project Introduction**

  

In this project I'll be dividing and grouping all individual customers of a grocery business into clusters based on shared common characteristics. This will be extremely beneficial to the business to formulate better marketing strategies and also understand their customer's needs and wants and cater services in a more personalized manner.

## **Project Overview**

  

* Grouped customers into clusters based on shared characteristics between them using unsupervised learning (K-Means clustering).
* Cleaned, explored and manipulated the entire data extensively on Python to make it usable for our use case.
* Engineered new features as and when necessary in accordance with our clustering requirements.
* Was able to extract meaningful insights from the data for each cluster that can help make efficient yet effective business decisions.
* Used K-Means clustering with optimal number of clusters that we were able to derive using elbow method.
* Used visualizations extensively to explore and visually interpret the data.

## **Potential Uses**

  

* Can help formulate better marketing strategies.
* Can help the business save money by making better and effective use of the marketing budgets.
* Can help the company gain a competitive edge over rival businesses.
* Can help to procure and develop better products by having a better understanding of the customer's needs and wants.



## **Data Cleaning**

* Removed insignificant features after analyzing descriptive stats.
* Engineered new features from existing features in accordance with our project objective.
     - Number of days customer is registered for
     - Customer age at max registration year
     - Customer Seniority
     - Couple or not
     - Total number of children
     - Total spend
     - Total campaigns accepted
* Simplified features to better fit our clustering.
* Removed outliers after analyzing boxen plots of relevant features.

## **Data Pre-Processing**
* Label Encoded relevant features.
* Scaled the data using standard scaler.
* Plotted and analyzed correlation matrix for better understanding. ![image1](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/1.png)

## **Clustering**

* Derived optimal number of clusters with elbow method by distortion score. ![image2](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/2.png)
* Grouped data into 4 fairly distributed clusters using K-Means clustering with relevant features. ![image3](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/3.png)

## **Data Exploration**

* Income and Total Spend with cluster info on scatter plot. ![image4](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/4.png)
We see that:
     -   Cluster 0: Average Income and Average Spending
     -   Cluster 1: Low Income and Low Spending
     -   Cluster 2: High Income and High Spending
     -   Cluster 3: Below Average Income and Below Average Spending
* Income relationship with our clusters. ![image5](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/5.png)
We can clearly interpret that Cluster 2 is our highest income group followed by Cluster 0 and then Cluster 3 and 1.

* Total Spend relationship with our clusters. ![image6](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/6.png)
We can clearly interpret that Cluster 2 is our highest spending group followed by Cluster 0 and then Cluster 3 and 1.

* We checked spending stats for each individual items with clusters. We were able to conclude:
    - Cluster 2 has the highest spending on Meat comparatively.
     - Cluster 0 has a high spending on Wines comparatively.
      - Cluster 3 has spent quite a lot on Gold comparatively.
      - Cluster 1 has the least spending but they have shown some interest towards Gold comparatively.

* Age groups relationship with our clusters. ![image7](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/7.png)
We can see that:
    -   Cluster 1 which groups our worst customers has the highest concentration of young customers (20-35 years).
    -   Cluster 2 which groups our best customers has a higher ratio of customers between 35 to 65 years.
    -   Cluster 3 has the highest ratio of 35 to 50 year olds.
    -   Cluster 0 has a high ratio of 50-65 year olds.

* Relationship of children with our clusters. ![image8](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/8.png)
We can see that:

    -   Cluster 2 which group our best customers has the highest ratio of 0 children and it looks very significant comparatively.**
    -   Cluster 3 has a high ratio of 2 children.
    -   Cluster 0, 1 and 3 has a high ratio of at least 1 children.

* Relationship of education with our clusters. ![image9](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/9.png)
We can see that:

    -   Cluster 1 has the highest ratio of Undergraduates comparatively.
    -   Cluster 3 and 0 both have a significantly higher ratio of Postgraduates.
    -   Cluster 2 majorly consists of Graduates and Postgraduates.
* Relationship of deals purchased with discount with our clusters. ![image10](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/10.png)
     - On an average Cluster 2 has the lowest number of purchases made with discount.
     - Cluster 0 has the highest number of purchases made with discount.

* Relationship of total number of campaigns accepted with our clusters. ![image11](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/11.png)
Total number of campaigns accepted is uniform with our best to worst clusters which makes it seems like customers were grouped similarly and specifically targeted with campaigns by the business in the past prior to our investigation.

* Relationship of older and newly registered customers with our clusters. ![image12](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/12.png)
We can see that:

    -   Cluster 0 and 3 has a higher ratio of old customers.
    -   Cluster 2 has a high ratio of newer customers comparatively.

* Relationship of living as a couple or alone with our clusters. ![image13](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/13.png)
We see that the ratio of couple or not are fairly distributed among all our clusters.

* Relationship of number of web visits per month with our clusters. ![image14](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/14.png)
We can see that:

   -   Cluster 2 on a average has the lowest number of Web visits per month.
   -   Cluster 1 on an average has the highest number of Web visits per month followed by Cluster 3 and 0.

* Relationship of number of purchases made through website with our clusters. ![image15](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/15.png)
We can see that:

    -   Cluster 1 on an average has the lowest number of web purchases.
    -   Cluster 0 on an average has the highest number of web purchases followed by Cluster 2 and 3.

* Relationship of number of purchases made directly through store with our clusters. ![image16](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/16.png)
We can see that:

    -   Cluster 1 on an average has the lowest number of store purchases.
    -   Cluster 2 on an average has the highest number of store purchases followed by Cluster 0 and 3.

* Relationship of number of purchases made through catalogue with our clusters. ![image17](https://raw.githubusercontent.com/rishi5565/customer-segmentation-unsupervised-learning/main/Images/17.png)
We can see that:

    -   Cluster 1 on an average has the lowest number of catalogue purchases.
    -   Cluster 2 on an average has the highest number of catalogue purchases followed by Cluster 0 and 3.

## **Conclusion**

After going through all the infomation above, we can conclude the profiling of customers in the following way:

-   **Cluster 0:**
    
    -   Has average income and average spending
    -   Likes to buy wines
    -   Relatively older
    -   Has atleast 1 children
    -   More educated
    -   Likes to make purchases with discounts
    -   Are generally older registered customers
    -   Likes to purchase from website
-   **Cluster 1:**
    
    -   Has least income and least spending
    -   Has shown interest towards gold comparatively
    -   Relatively younger
    -   Has atleast 1 children
    -   Least educated comparatively
    -   Visits website very frequently
    -   Low number of purchases
-   **Cluster 2:**
    
    -   Has highest income and spending
    -   Loves to buy meat
    -   Spans all ages generally but lacks young customers
    -   Has no children mostly
    -   Fairly educated
    -   Does not make much purchases with discounts
    -   Are generally newly registered customers
    -   Does not visit website much
    -   Loves to purchase from store and catalogue
-   **Cluster 3:**
    
    -   Has below average income and spending
    -   Likes to buy gold comparatively
    -   Relatively middle-aged
    -   Has atleast 1 or more than 1 children
    -   More educated
    -   Are generally older registered customers
    -   Visits websites quite frequently

Data Source: [Link](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)

### [Note]:  _**Please refer to the Project Notebook file for all the detailed in-depth information regarding this project. The above information is just a brief summary of the project.**_

Thank You,

Rishiraj Chowdhury ([rishiraj5565@gmail.com](mailto:rishiraj5565@gmail.com))
