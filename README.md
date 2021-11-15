# Amazon_Vine_Analysis

## A) Overview

Analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. In this project, the reviews dataset for gaming product has been selected to to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Further analysis includes useing PySparkto determine if there is any bias toward favorable reviews from Vine members in the selected dataset. A summary of the analysis is presented.

## B)Resources

Data Source: Amazon Review datasets, Product: Video Game (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
Software: Google Colab Notebook, PostgreSQL 11.9, pgAdmin 4, AWS

## C) Results

- Total number of paid vine reviews: 94

- Total number of 5-star paid vine reviews: 48

- Percentage of 5-star paid vine reviews: 51 %

- Total number of unpaid vine reviews: 40471

- Total number of 5-star unpaid vine reviews: 15663

- Percentage of 5-star unpaid vine reviews: 39 %

## Summary

Out of 94 reviews of the members in Vine program, 48 have voted 5 star for the product of this study. This accounts for 51 % of reviews given as 5 stars. In comparison, out of 40471 members who did not participate in vine program, 15663 (39%) have given 5 stars review to the product. The result of this comparison suggests that there is a there is to some extent bias toward favorable reviews from Vine members.
Futher statistical study can be designed to run the T-test to understand the significance of the diffrence between the entire dataset and the sample of 5 stars rating.
