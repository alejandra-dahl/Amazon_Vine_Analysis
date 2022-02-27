# Amazon Vine Analysis

## Overview

Manufacturers and publishers receive reviews for their products throught the Amazon Vine program service. SellBy, a company that sells on Amazon, pays a a fee to have Amazon Vine members review their products. This helps them build credibility and a customer base.


### Purpose

The purpose of this analysis was to compare Vine and non-Vine reviews to determine if their is any bias toward favorable reviews, coming from Vine members.


## Results

The dataset that was chosen for this analysis can be found [here](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Jewelry_v1_00.tsv.gz) This dataset consisted of Amazon reviews for jewelry. Using this dataset, the following questions were addressed in the analysis.

![image](https://user-images.githubusercontent.com/90485451/155902838-3555b944-6c26-47f3-a88f-9c12cb6804ef.png)


  **- How many Vine reviews and non-Vine reviews were there?**
  
     In order for this analysis to have the most credibility, the dataset was filtered into a dataframe to show only reviews 
     
     that were more likly to be helpful and avoid division by zero errors later. From there, DataFrames were created to retrieve 
     
     all the rows where a review was written as part of the vine program ('Y') and reviews that were non-Vine. 
     
     There were a total of **21 vine reviews** and **7,689 non-vine reviews**. 

  **- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
  
      From those 21 vine rviews, the dataset was then filtered in another DataFrame to retrieve Vine reviews 
      
      that had a 5-star review. There were a total of **11 5-star vine reviews**. The same was done for non-Vine reviews which 
      
      had a total of **4,444 non-vine 5-star reviews.**

  **- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
  
  Percentages were then calculated for each result. There were - 
  
      57.8% of unpaid reviews with 5-stars
  
      52.38% of paid reviews with 5-stars
      
      
![image](https://user-images.githubusercontent.com/90485451/155904174-ee65111e-f748-4439-b21b-8aead228278a.png)


## Summary

The results show that there doesn't seem to be much bias between paid and unpaid reviews - as seen from 5 star reviews. It was also interesting to see that there were more non-Vine reviews than paid reviews. This shows that the product is very favorable in the marketplace and the seller could probably go without paid reviews.

An additional analysis that could be done in the future is look at reviews that are 3-stars or less and seeing how many of those are paid vs non-paid.
