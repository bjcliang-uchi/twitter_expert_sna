# Social Network Analysis on Twitter-based Policy Expert Networks
Chen Liang

## Parallel Scraping
**parallel_follower_following.ipynb**
Using S3 and PyWren to scrape all follower/ following information

**scrape_tweets.ipynb**
Using S3 and PyWren to scrape at most 300 pages of tweets for each user

## Sequential Scraping
**scrape_citations.ipynb**
Automatically search each expert’s name on Google Scholar and save all search results. I then manually match experts to search results based on their past experience.

## Data Integration
**check_account.ipynb**
This notebook integrates different sources of data and checks if any user needs to be rescraped. I rescrape an user if the total numbers of follower/ following accounts we obtain are significantly different from the true numbers of followers/ following accounts based on the user profile information.

**data_integration.ipynb**
I obtained multiple dataset from Harvard Dataverse and used them to identify whether an account is related to Federal Government agencies, Congress, and news outlets. This notebook integrates the datasets and classify accounts who either follow and are followed by our targeted experts.

## Data Analysis
**data_exploration.ipynb**
This notebook explores our data from a non-network perspective. It summarizes the time when experts join Twitter, the distribution of followers/ following numbers, the distribution of citation index and  its correlation with other variables.

**sentiment_analysis.ipynb**
Load tweets data. Apply SentimentIntensityAnalyzer and MultiProcessing to calculate the sentiment scores for each tweet. Calculate average sentiment scores for each expert.

**regression_models.ipynb**
Integrate data into analyzable format: calculate the components of followers/ following accounts; construct networks to calculate centrality; code job titles; calculate tweeting frequency; ran multiple regressions.

**graph.ipynb**
calculate Gini coefficients for centrality measures; visualize all needed network graphs.
