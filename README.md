

# Employee reviews NLP and Predictive model project



## Goals:
Employees are looking for a good company to work at, meanwhile companies are trying to retain good employees because hiring process are costly and take long time. It is also taking time for the new employee to learn the technology and process using in a company. Therefore, it is important to know for employees to learn about the culture of the company before they consider joining. It is also important for the companies to understand how they can keep employees happy so they can perform better in their job and consider being with them for long time. We will use employee’s reviews for the 5 big companies to analyze the reviews, build a predictive model and find the relationship between words used in the reviews and ratings.


### Executive Summary:

The data includes reviews from employees of Amazon, Apple, Facebook, Google, Microsoft, and Netflix. Following are the number of reviews for each company used for this project.
Amazon 26,430
Microsoft 17,930
Apple 12,950
Google 7,819
Facebook 1,590
Netflix 810
There are 67,529 rows and 17 columns in the data frame. The columns are (company name, location, date of the review, job title, summary, pros, cons, advice to management, overall rating, work balance rating, culture values rating, career opportunities rating, compensation benefits rating, senior management rating, helpful count and link to the review.)

First we explored the data and get some insights about the dataset, then we tried to see the distribution of ratings for each company, we came to understand some companies have more less than 5 stars than other companies, for example Facebook reviews are mostly 5 star and very less 1-4 star compare to Netflix and Amazon, which might indicate that people who works at Facebook might be happier with their job and Facebook might have better work and culture environment compared to Amazon and Netflix.  

After that, we run some word clouds on summary column to show the importance of each word by size and color. These words could be related to pros and be positive word or cons and negative word about the company. We set the perimeter to 40 words so we can get only the 40 most important words. There are similar words across all companies with different levels of importance which means, mostly employees have similar opinion while writing review for a company.
After that we started working on building predictive model so that our model can predict if an unseen review comes under positive or negative category. To do so we did some data cleaning and feature engineering which include, for this model we only needed the pros, cons and overall rating columns. 
We changed the rating column to 0 and 1, any rating 3 or more to be 1 and 2 or less to be 0. Then we used regular expression operations to get a clean data, we also changed the data to lower case and tokenized. Afterword to improve our model we removed the English stop words and then normalized our data using porter steamer and add all rows to one blog of text in sting format separated by commas. 
After having our clean data ready we train test split our data and built a pipeline and add nonvectorized and logistics regression model. 

The next step would be to Gensim model and find the correlation between the words in reviews and ratings and understand the relationship between them. 


### Conclusions and Recommendations:
In conclusion we came to understand employees are looking for similar values when joining a company, Facebook and Google might have more employee friendly culture than Amazon, Netflix, Microsoft and Apple. However, the result might change if we could collect more data for companies and make sure the number of reviews for each company are the same. 
We also have list of words that are important to employees with their importance level so the companies can focus those aspects and consider and improve them in their new management strategies. We also built a model that can predict if a review is positive or negative which can be used for companies to analyze their employees’ feedback without making them uncomfortable with giving stars between 1-5 if the survey is not anonyms. 
  
The next step for this project would be to find and identify the most important words in pros (positive) and cons (negative) reviews and find the relationship between positive and negative words with the number of starts provided so that we can understand how much each word has influence to change the star ratings.   


[Have Question? ](https://roymansoor.com)