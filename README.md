# Customer-Segmentation-of-Retail-Industry


# Objective
The purpose of the report is to propose an RFM based clustering technique and to classify customers of
a national convenience store chain into segments. Business recommendation are proposed based on the analysis result.



# Dataset
• Transactional data from the loyalty card scheme including 3,000 customers' purchase record in 6 months

• The data contains time,customer id,total spend, total qty.
 
 
 # Feature Description
 RFM is one of the most widely used methods to perform customer segmentation due to its simplicity and availability.
 On top of that, the report takes other behavrioul data into consideration to better identify customer groups.
 
 
 **Recency**:The count of days since the individual’s last transaction. The feature was generated from “purchase_date” of the dataset.
 The count of the days between the last purchase date and the snapshot date.

 **Frequency**: The count of times an individual has purchased from the brand in the six months.
 
 **Monetary**: Ths sum of an individual's transaction amount.
 
 **Length**: The duration between one's first and last transaction date. It provides further information on the stage of customer journey.
 eg. new comers may have lower length but it's worth observing its monetary and frequency values.
 
 **Average spend per shop**: The average amount of one's spend per transaction.
 
 **Count of unique product id**: The count of unique product an individual has bought.
 
 


# Feature Engineering
• Due to high correlation between features is likely to decrease the performace of the clustering (curse of the dimensionality)

• `PCA` (Principle component analysis) is employed to reduce the dimension

• 95% information is retained with 4 PCA components


# Clustering
• Apply `KMeans` from Sklearn

• Using `silhouette_score` to decide the value of k


# Segmentation Result Analysis
• Use `df.describe()` to print the overall information of each cluster 

• Apply seaborn to visualize the customer composition in pie charts

• Visualize the difference between groups with box plots



# Customer Pen Portraits
**GROUP 0 - Low Contribution Loyal**: The group of people only come for certain exclusive products. Price sensitive. 

**GROUP 1 - At Risk**: Haven't shown up in the shops for a while. Less frequency and low monetary value but high average spending per visit.
They might have negative shopping experience with the brand leading to the less visits.

**GROUP 2 - Low Value Lapsed**: They haven't shown transaction activities for a long time who may have already exited from the customer base.

**GROUP 3 -High Contribution Loyal**: Highest monetary, longer relationships with the brand.
Tend to make less frequent trips to the shops but whenever they shop, they spend much more than average people do.


**GROUP 4 - High Contribution Active**: Highest visit frequency, high monetary value. They're in favor of multiple top-up shops instead of having main grocery shoppings.


# Business Recommendations: 
**Priority for future marketing campaigns**

**1. Low Contribute Loyal**: 60% of the customers belong to the group. Increase their average spending will contribute significantly in the revenue.

**Proposals**: Offer conditional promotions (eg. 3 for 2) to stimulate spending

**2. At Risk customer**: The group has high average spend, need to know what caused their less frequent visit. 

**Proposals: Personalized vouchers. Customer survey form to understand more about their dissaticfations. 
 
 
 
 
 
 




