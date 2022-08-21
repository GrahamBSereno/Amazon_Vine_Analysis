# Amazon_Vine_Analysis

## Purpose
Perform analysis on Amazon reviews to assess whether 'Vine' loyalty program members have a bais towards favorable reviews when compared to non-'vine'-loyalty member customers.

## Steps
1. Analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
2. Access approximately 50 datasets each containing reviews of a specific product, from clothing apparel to wireless products. Pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 
3. Use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Results
Vine Loyalty Member Reviews Total
- 90 (Reference line 14 in the below Results Output screenshot)

Non Loyalty Member Reviews total
- 37,831 (Reference line 15 in the below Results Output screenshot)

5 Star Vine Loyalty Member Reviews Total
- 44 (Reference line 18 in the below Results Output screenshot)

5 Star Non Vine Loyalty Member Reviews Total
- 14,704 (Reference line 19 in the below Results Output screenshot)

Percentage of Vine Loyalty Member 5 Star Reviews
- 48.89% (Reference line 22 in the below Results Output screenshot)

Percentage of Non-Vine Loyalty Member 5 Star Reviews
- 38.87% (Reference line 23 in the below Results Output screenshot)

### Results Overview (Jupyter Notebook Screenshot)
![](https://github.com/GrahamBSereno/Amazon_Vine_Analysis/blob/main/ResultsOverview.png)


### Summary
- As shown in the above analysis there is a slight positivity bias for reviews in the Vine Loyalty Program.
  - Approximately 49% of Vine Loyalty Member Reviews are 5-Star which is higher compared to Non-Vine Loyalty Members (39%).

### Additional Analysis Proposal
- To further test this conclusion, the seasonality should be taken into account to consider how moods of customers impact 5-star rating percentages.
  - Are Non-Vine Loyalty Members likely to rate higher around Christmas time? 
  - Key holiday products could be analyzed for 5-star rating volume between Loyalty and non-Loyalty members.
