# Amazon_Vine_Analysis

_Analysis with Pyspark on Amazon Web Services_

Note: Password from Amazon_Reviews_ETL.ipynb file is deleted for safety reason. 
(ETL File needs database password to create tables again)

## Project Overview

The purpose of this analysis is to determine if there is any bias in reviews favoring Vine from Vine members. 
Amazon Vine program is a service that allows manufacturers to have reviews posted on Amazon for their pre-release items, for an additional fee.

## Resources

The data source used for the analysis is
-   [Amazon Vine Reviews for outdoors items](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Outdoors_v1_00.tsv.gz)

## Deliverable
-   ETL on Amazon Web Services RDS and access via pgAdmin[Amazon_Reviews_ETL.ipynb](https://github.com/gopivasanth/Amazon_Vine_Analysis/blob/f45a2d89dd2e1dc1893c7ea554afcda4c359cc0b/Amazon_Reviews_ETL.ipynb)
- Data imported to AWS RDS
![RDS Image](https://github.com/gopivasanth/Amazon_Vine_Analysis/blob/314d0652f5a53cc89ca13a94f502dad2cc966302/pgAdmin_RDS.png)
-   Vine Review Analysis on Google Colab [Vine_Review_Analysis.ipynb](https://github.com/gopivasanth/Amazon_Vine_Analysis/blob/f45a2d89dd2e1dc1893c7ea554afcda4c359cc0b/Vine_Review_Analysis.ipynb)

## Results

In this analysis the Amazon Vine reviews that have more than 20 total votes and the percentage of helpful votes is equal or greater than 50.

_**How many Vine reviews and Non-Vine reviews were there?**_

There were
-   107 Vine reviews &
-   39869 Non-Vine reviews.

_**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**_

There were
-   56 five stars Vine reviews
-   21005 five stars Non-Vine reviews.

_**What percentage of Vine reviews were 5 stars? What percentage of Non-Vine reviews were 5 stars?**_

-   52.34 % of Vine reviews were 5 stars
-   52.69 % of Non-Vine reviews were 5 stars

![Results](https://github.com/gopivasanth/Amazon_Vine_Analysis/blob/314d0652f5a53cc89ca13a94f502dad2cc966302/Vine_Review_Analysis.png)

## Summary

The purpose of this analysis is to analyze and determine if there is any bias toward favourable reviews from Vine members. 
- The analysis of reviews that have more than 20 total votes and the percentage of helpful votes is equal or greater than 50. This selection was made in order to pick reviews that are more likely to be helpful.

Positivity bias for reviews in the Vine program

- The analysis of 5-star reviews within conditions mentioned show that there is NO positivity bias for reviews in the Vine program**. The results show that percentage of 5 stars Vine reviews is 52.34% and percentage of 5 stars Non-Vine reviews is 52.69%.  **Non-Vine reviews**  have slightly  **higher percentage**  of the 5 stars reviews

- The results show that there could be positivity bias for reviews in the Vine program, when looking from 1 and 2-star reviews perspective.
