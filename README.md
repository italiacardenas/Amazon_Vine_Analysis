# Amazon Vine Analysis

## Analysis Overview
The purpose of this analysisis took look at Amazon reviews written by memeber of the paid Amazon Vine program. A small fee is paid by companies such as Sellby to Amazon Vine members, requiring them to publish a review. Out of the 50 datasets available, review left for books were chosen. 

PySpark was used to perform an ETL process that extracted, transformed and connected to an AWS DS instance. The new data was then loaded into pgAdmin. In order to determine whether there were bias toward favorable reviews left for books from Vine members.


## Sources
- [Book Reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Books_v1_02.tsv.gz)
- Google Colab Notebook, pgAdmin 4, AWS

## Results

### Vine Book Review Results
Interestingly enough, Book Reviews were not being made by Vine Members. This means that companies are not looking to pay Vine Members to leave book reviews. 
<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/paid_reviews.png"> 


### Unpaid Book Reviews Results
Books Reviews were solely written by unpaid shoppers. Out of 40,387 reviews left, 60% of them were 5-star reviews. This means that the majority of 5-star reviews were left organically and not influenced by a pay. It also means that Amazon has a great book selection that shopeprs are genuinely enjoying.
<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/unpaid_reviews.png"> 


## Summary
The results suggest that Books are being bought by people who appreciate reading and are probably sticking to the genres they are guaranteed to like. Although 40%of the reviews are unacocunted for, because 60% of the reviews left 5-stars, it is safe to say so. Additionally, 4-star reviews could also be accounted for and combined with the 5-star reviews to determine whether there is a significant amount of positive reviews left for books on Amazon.
