# G1S8_-Project-2_Python-for-DS-
Data cleaning,exploratory analysis,model building ,PCA and cluster analysis on rent_runaway data

Machine Learning-Unsupervised

Domain:-E Commerce
Business Context:-
1.Customer segmentation is one of the most important marketing tools at your disposal, because it can help a business to better understand its target audience.
2.Segmentation can be based on the customer’s habits and lifestyle, in particular, their buying habits. Different age groups, for example, tend to spend their money in
 different ways, so brands need to be aware of who exactly is buying their product
3.Segmentation also focuses more on the personality of the consumer, including their opinions, interests, reviews, and rating. Breaking down a large customer base into more
manageable clusters, making it easier to identify your target audience and launch campaigns and promote the business to the most relevant people.

Dataset Description:
The dataset contains measurements of clothing fit from RentTheRunway. RentTheRunWay is a unique platform that allows women to rent clothes for various occasions. 
The collected data is of several categories. This dataset contains self-reported fit feedback from customers as well as other side information like reviews, ratings, product categories, catalog sizes, customers.

Project Objective:-Based on the data,segment similar users and items into suitable clusters and analyze the clusters.

Steps undertaken:-
1)Loaded data set and checked the basic info. There were 16 columns and 192544 rows.
2)Data Cleaning and EDA:- checked for duplicate records and dropped redundant columns.
3)Defined function for converting string data into float type for variables height and weight
4)Checked for missing values and bust size,body type replaced by the mode and height,weight,rating, age replaced by the median.
5)Checked for statistical summary for both numeric and categorical data
6)Checked for outliers and used IQR(Inter quartile range) method to remove them/minimise it.
7)Checked the didtribution for different categories in column rented for
8)Prepared the Data for model building
a)encoded the categorical varioable using Label encoder.
b)Using standard scaler scaled data-
c)Applied PCA Principal Component Analysis to find out how many variables should be used so that 90-95% of data is explained-8 is optimum
d)PCA model fitted with scaled variables.
e)K-mean clustering done to segment the data..from elbow plot 4 clusters were optimal
f)Computed silhoutte score for evaluating the quality of K means clustering.
g)Applied agglomerative clustering model and using the optimal K value--was 3
h)Performed cluster analysis by doing a bivariate analysis between cluster labels and different features
