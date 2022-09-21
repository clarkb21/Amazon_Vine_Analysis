# Amazon_Vine_Analysis

## Purpose
- The purpose of this project is to demonstrate skills using Spark, Google Colab, and Big Data information. 
- Data was extracted from Amazon Web Services S3 Buckets into a Google Colab Notebook, transformed using PySpark, and then loaded into a PostgreSQL database.
- The main purpose of the challenge was to determine if there is any bias with Vine reviewers versus non-Vine members.

## Project Overview
- Key concepts on "Big Data" were introduced, including Spark, Hadoop, Amazon Web Servies (AWS), and MapReduce.
- Google Colab Notebooks were used to utilize Spark dataframes and functions. 
- The Natural Language Processing pipeline was introduced, including the process to tokenize data, stop words, and term frequency-inverse document frequency weighting.


### Challenge Overview
- A large dataset was extracted from an AWS bucket through an AWS RDS instance. The data was then transformed and loaded into a PostgreSQL database using pgAdmin 4.
- Using PySpark, queries were executed to determine the number of reviews, number of 5 star reviews, and percentage of 5 star revies for Vine reviewers and non-Vine reviewers.
- That information was then used to determine if there is any bias in the reviews from Vine members. 

## Results
**1. How many Vine reviews and non-Vine reviews were there?**
- Vine members had a total of 24,171 reviews in the dataset. 
- Non-Vine members had a total of 3,456,395 reviews.

**2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
- Vine members had 9,833 5-star reviews.
- Non-Vine members had 1,898,455 5-star reviews.

**3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
- Vine members had 5-star reviews approximately 40.7% of the time. 
- Non-vine members had 5-star reviews approximately 54.9% of the time. 

![image](https://user-images.githubusercontent.com/104038813/191538395-f55a680b-0307-4660-ba4f-29377f1f1296.png)

## Summary
- Based on the results, Vine members are less likely to rate items with 5-star reviews than their non-member counterparts. 
- Vine members, who do not have to pay for the items and are striclty there to provide accurate reviews, only gave 5-star reviews 40% of the time. 
- Non-Vine members, who purchased the items because they wanted or needed the item, gave them 5-stars over half the time.
- Vine members do not have favorable bias towards these items solely because they are a Vine review member.

#### Additional Analysis
- With the given dataset, another analysis that could be done to show the rate of 5-star reviews would be to look at the Verified purchase column. 
- Vine members do not pay for the items, but receive them solely to give accurate reviews. 
- An additional query could have been done to filter on the verified purchase column for non-Vine members to see the difference between 5-star reviews for customers who actually bought the item and those that did not. 

## Resources
- Data Source: "https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Sports_v1_00.tsv.gz"
- Software:  pgAdmin 4, Google Colab Notebook, PySpark
- MSU Bootcamp Spot Module 16: https://courses.bootcampspot.com/courses/2508/assignments/31932?module_item_id=637495


