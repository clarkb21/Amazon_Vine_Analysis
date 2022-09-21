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



## Summary


## Resources
- Data Source: "https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Sports_v1_00.tsv.gz"
- Software:  pgAdmin 4, Google Colab Notebook, PySpark
- MSU Bootcamp Spot Module 16: https://courses.bootcampspot.com/courses/2508/assignments/31932?module_item_id=637495


