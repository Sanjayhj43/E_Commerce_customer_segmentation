# E_Commerce_customer_segmentation

Analysis of an E-Commerce customer database that lists purchases made by over 4000 customers over a period of one year, developed a model that allows to anticipate the purchases that will be made by a new customer, during the following year, from its first purchase.

# Abstract
A key challenge for e-commerce businesses is to analyze the trend in the market to increase their sales. The trend can be easily observed if the companies can group the customers; based on their activity on the e-commerce site. This grouping can be done by applying different criteria like previous orders, mostly searched brands and so on.

# Problem Statement
Given the e-commerce data, use k-means clustering algorithm to cluster customers with similar interest.

# Dataset Information

Column	Description
Cust_ID	- Unique Numbering of Customers
Gender	- Gender of Customer
Orders  - No. of Past orders placed by the customers

Remaining 35 features (brands) contains the number of times customers have searched them.

# Work Flow
First Import the necessary libraries needed for the project. Below are the libraries that I have used

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

from sklearn.preprocessing import MinMaxScaler

from sklearn.metrics import silhouette_score

from sklearn.cluster import KMeans

from yellowbrick.cluster import KElbowVisualizer

Load the dataset using pandas.

Understand the data with basic statistics, info, total records, features and their data types also number of null values.

Perform the data cleaning techniques like treating the missing values.

Visualize the data with the help of Matplotlib or Seaborn to get better understanding of the features.

In my project I have used Seaborn's

Boxplot(To visualize the Outliers present in the data)

Barplot (To get to 10 customer ID based on Total searches)

Countplot (To get gender count and Prior orders count)

Heatmap (To find the Correlation)

Histogram (To get know how the data is distributed)

Below are some of the charts that I have plotted

![image](https://github.com/Sanjayhj43/E_Commerce_customer_segmentation/assets/114797457/31fa4074-e3ea-48a3-94f7-4905f303ce49)

![image](https://github.com/Sanjayhj43/E_Commerce_customer_segmentation/assets/114797457/d8bfa3b2-075a-4340-a077-bec2d282f3c3)

Perform the data scaling using minmaxscaler and data will be scaled between 0 and 1.

Implement the Elbow method or Silhouette method to find the optimum number of K. Also visualize them with plots.

![image](https://github.com/Sanjayhj43/E_Commerce_customer_segmentation/assets/114797457/701781d3-107c-4a3e-80a6-f7f8464e67ef)

After getting optimum K value use it as number of clusters and perform the model fit.

The model will provide the output with different clusters.

Analyed each clusters using visualization techniques to find the insights.

![image](https://github.com/Sanjayhj43/E_Commerce_customer_segmentation/assets/114797457/db15897a-e49d-41a3-8f70-3b76ee03c72c)

Refer python file for complete source code for this project



