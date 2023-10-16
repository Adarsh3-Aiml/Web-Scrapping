# Web Scraping for Indeed.com and Predicting Salaries
<img src="http://imgur.com/1ZcRyrc.png" width="60">

## Business Case Overview
You're working as a data scientist for a contracting firm that's rapidly expanding. Now that they have their most valuable employee (you!), they need to leverage data to win more contracts. Your firm offers technology and scientific solutions and wants to be competitive in the hiring market. Your principal wants you to determine the industry factors that are most important in predicting the salary amounts for these data. To limit the scope, your principal has suggested that you focus on data-related job postings, e.g. data scientist, data analyst, research scientist, business intelligence, and any others you might think of. You may also want to decrease the scope by limiting your search to a single region.

Goal: Scrape your own data from a job aggregation tool like Indeed.com in order to collect the data to best answer this question.

## Approach

## Data Collection:
- Web-scraping: BeautifulSoup, Request

## Data pre-processing:
- Feature engineering of keywords contained in job-title, and convert salaries to same format
- NLP techniques (TfidfVectorizer) to allow Job Summary to be used as input into model

## Modelling:
- Linear Regression to predict salary of job based on features collected from job postings
- Then classification techniques were compared (Bagging, Random Forest, Gradient Boosting) to classify High vs Low salary.
- Features added piecemeal to measure the impact of each feature on overall model performance

## Evaluation:
- ROC curve used to visualise best-performing model
