# Amazon Vine Analysis

## Overview of the analysis:
 
This analysis is to create a larger project to analyze Amazon reviews written by members of the paid Amazon Vine program. Having access to 50 datasets, the Music dataset was chosen to analyze. Using PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and lod the transformed data in pgAdmin. The end result is to determine if there is a favorable review from Vine members. 

## Results

### How many Vine reviews and non-Vine reviews were there?

* There were a total of 7 paid Vine reviews found in our music dataset as seen in the below image. 

![vinepaid_reviews.PNG](https://github.com/nyoung246/Amazon_Vine_Analysis/blob/main/Resources/vinepaid_reviews.PNG)

* And a total of 105,979 unpaid Vine reviews found in our music dataset, as seen in the below image.

![vineunpaid_reviews.PNG](https://github.com/nyoung246/Amazon_Vine_Analysis/blob/main/Resources/vineunpaid_reviews.PNG)


### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

* There was a total of 67,580 Vine reviews found in the dataset, as seeen in the below image.

![5star_vinereview.PNG](https://github.com/nyoung246/Amazon_Vine_Analysis/blob/main/Resources/5star_vinereview.PNG)

* And a total of 0 non-Vine reviews found in the dataset, as seeen in the below image.

![5star_nonvinereview.PNG](https://github.com/nyoung246/Amazon_Vine_Analysis/blob/main/Resources/5star_nonvinereview.PNG)

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

* There was a 63.77% of 5 star Vine reviews found in the dataset, as seen in the below image.

![percent5star_vine.PNG](https://github.com/nyoung246/Amazon_Vine_Analysis/blob/main/Resources/percent5star_vine.PNG)

* And a 0% of 5 star non-Vine reviews found in the dataset, as seen in the below image.

![percent5star_nonvine.PNG](https://github.com/nyoung246/Amazon_Vine_Analysis/blob/main/Resources/percent5star_nonvine.PNG)

## Summary

The analysis shows that there are a total of 7 paid reviews with 0% 5 star non-Vine reviews,as opposed to 67,580 unpaid reviews and 63.77% 5 star Vine review. As the unpaid and Vine reviews were substantally more than the paid and Vine, we are to conclude that there is no positivity bias for reviews in the Vine program. This being said, it may not mean that the Vine program will have no positivity bias in the future as there were still 7 paid reviews found in the dataset.

An additional analysis that could be conducted with the Music dataset is to include the analysis of other star ratings. This would give us a true picture of whether there is positivity bias in the Vine program. As other star ratings like a 4 star rating is also a very good rating and could show positivity bias in the program. Only conducting a 5 star review analysis limits our capability to capture all the details in between, and the reality could be a completely different conclusion.
