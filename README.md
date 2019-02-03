# Instagram_Analytics
## Is a Picture Worth a Thousand Words?  
This project was done as part of the "User Generated Content Analytics" course

Total number of team members : 4

## Summary Steps: 
* On Instagram, choose the National Geographic (natgeo) page (do not use hashtags). Write a scraper or use the Web Scraper to extract (i) image URLs (do not extract video URLs, it may end up costing you a lot of money to run analytics on video), (ii) post caption (the text description of a post), (iii) # likes and (iv) # comments. You don’t need actual comments for this assignment. Scrape 250-500 image posts. 
* Using the image URLs, obtain image labels from Google Vision cloud (you will have to create an account with Google to get your credentials as a json file, though the first $300 are free, which should be more than plenty for this assignment). You will need to write a script to access the Google Vision API. 
* Create a metric for engagement by using a weighted sum of # likes and # comments. However, first normalize # likes and # comments such that they both have values between 0 and 1. You can scale the # likes by dividing by the maximum # likes (for a post) in your data and do the same for # comments, so that # likes and comments will be in the range [0,1]. Now create an engagement score = .4*# likes (normalized) + .6*# comments (normalized). Define High (1) and Low (0) engagement based on whether the engagement score is above or below the median value.  
* Run a logistic regression with Engagement (binary) as the dependent variable, and the image labels as independent variables. 
* Perform topic modeling (LDA) on the image labels. Choose an appropriate number of topics. You may want to start with 5, but adjust the number up or down depending on the word distributions you get. LDA should produce two outputs: (i) A file showing which words load on which topics, and (ii) a file showing topic weights for each image. 

## Tools and Methods used:
* Octoparse - for scraping images
* Lift Calculation
* Natural Language Processing
* Word replacement
* Sentiment Analysis
* Cosine Similarity


