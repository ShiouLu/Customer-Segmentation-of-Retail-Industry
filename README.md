# Customer-Segmentation-of-Retail-Industry


# Objective
▪︎ The purpose of the project is to perform a customer segmentation on a transactional dataset provided by a convenience store chain.

▪︎ Based on the result, customer profile for each group is generated and business recommendation derived from the clustering results are also provided.



# Dataset
• Transactional data from the loyalty card scheme including 3,000 customers' purchase record in 6 months

• Two files were used to underpin the analysis: basket.csv and lineitem.csv
 
 
 # What's in the project
 • Data Cleansing in Python `pandas`
  
 • Feature Engineer - `PCA`
 
 • Perform Clustering using `KMeans`, `silhouette_score`
 
 • Visualize group difference with `Matplotlib`,`seaborn`
 
 
 
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
 
 




# Customer Pen Portraits
**GROUP 0 - Low Contribution Loyal**: The group of people only come for certain exclusive products. Price sensitive. 

**GROUP 1 - At Risk**: Haven't shown up in the shops for a while. Less frequency and low monetary value but high average spending per visit.
They might have negative shopping experience with the brand leading to the less visits.

**GROUP 2 - Low Value Lapsed**: They haven't shown transaction activities for a long time who may have already exited from the customer base.

**GROUP 3 -High Contribution Loyal**: Highest monetary, longer relationships with the brand.
Tend to make less frequent trips to the shops but whenever they shop, they spend much more than average people do.


**GROUP 4 - High Contribution Active**: Highest visit frequency, high monetary value. They're in favor of multiple top-up shops instead of having main grocery shoppings.



 
 
 
 
 
 




