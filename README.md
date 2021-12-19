# Amazon_Vine_Analysis
## Project Overview
The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine program. We will also be looking to determine if there is a review bias for Vine program items.  This analysis will be performed using the following tools: 
 - PostgreSQL
 - Python
 - Pyspark
 - Pandas
 - Data provided by Amazon containing user reviews provided by for products. 

### Data Cleanup
There were 104,975 reviews provided in the intial dataset. Of those reviews we're only looking at reviews that have a total vote count of 20 or more. This narrowed the dataset down to 1190. 

We filtered this data further by looking at reviews that had been voted helpful at least 50 percent of the time. From this point we were able to begin filtering Vine vs non Vine reviews. This brought us to a total of 1168. 

### Vine vs Non Vine Breakdown
Of the filtered dataset we can determine that there are:
![vine no](https://user-images.githubusercontent.com/88564212/146659353-5f4ef1a9-ec5a-4692-ba4a-f2d6af975b3c.png)
 - 1064 non Vine reviews. See above image for snippet of the non Vine review data set. 

![vine yes](https://user-images.githubusercontent.com/88564212/146659365-39951606-d557-4a47-ad1b-f8d49af46aae.png)
 - 4 Vine reviews. See above image for the entire Vine review data set. 
 
From here we wanted to determine the amount of 5 star reviews that each category receieved. 
 - Non Vine reviewers left 527 5 start reviews putting the overall rating at 49.53%
 - Vine reviewers left 1 5 star review with an overall rating of 25%



Obviously at this point we can see that the data provided to us will not be able to reliably tell us if we have a review bias with the numbers of the samples being vastly different. Ultimately to glean anything of value from this data set we would have to open up our criteria for what counts as a valid review to perform this analysis on. Alternatively we could seek out different data set that has more variety. 
