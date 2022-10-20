# Amazon_Vine_Analysis

## Overview of the Analysis of Amazon Vine Program

The purpose of this project is analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

We selected the video game dataset and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Using Pandas, we determined if there is any bias toward favorable reviews from Vine members in your dataset compared to non-Vine members (unpaid). Below is the summary of our analysis. 

## Results:

* How many Vine reviews and non-Vine reviews were there?

For this analysis we examined reviews of video games from the 50 datasets provided. Based on the records provided and those with greater than 20 reviews, there were 94 paid Vine member reviews and 40,471 unpaid non-member reviews. 

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

Of the 94 paid Vine member reviews, 48 (51%) had a rating of 5-stars. This is significantly different from the proportion of 5-stars provided by unpaid non-members where only 39% (n = 15,663) rated videos games 5-stars. 

![Screen Shot 2022-10-19 at 10 05 41 PM](https://user-images.githubusercontent.com/107972848/196841219-8afdc0cf-5233-4a8c-ae43-a21da4c10184.png)

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

As stated above, vine members more frequently (based on proportions) provided 5-star ratings for video games (51%) compared to unpaid non-Vine members who rated games at 39%. 

![Screen Shot 2022-10-19 at 10 10 58 PM](https://user-images.githubusercontent.com/107972848/196841084-f55f06ab-e0f6-4e0a-85ea-ef0402600f98.png)


## Summary:

* Is any positivity bias for reviews in the Vine program? 
* Any additional analysis to further support the results? 

Overall, paid Vine members seem to present more favorable reviews than non-Vine members. While the numbers are small, even a weighted average of the results would yield similar results. Additional analysis, using similar measure of central tendency were ran to see the 50% mark for the data (median) against the mean score. Similar to the previous results, vine members had a median rating of 5.0 for games compared to 4.0 for non-Vine members. Additionally, the average rating for vine members was 4.2 compared to the average rating from non-Vine members (3.35). 


![Screen Shot 2022-10-19 at 10 19 03 PM](https://user-images.githubusercontent.com/107972848/196840905-6b3848bf-c28f-49d6-8220-531c4aa5175b.png)
