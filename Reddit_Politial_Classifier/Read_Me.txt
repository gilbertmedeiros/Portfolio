Reddit Political Classifier

Goal: Based on reddit API data can you classify political posts source as Democratic or Republican leaning.

Process: 
    Scrape data from r/democrats and r/Republicans 'hot' page including text (title, comments and replies) and numerical data such as num of comments, time since post, num of replies etc.
    Clean and impute NLP (Natural Language) data to be used in a Random Forest model.
    Determine feature correlations and P-values along with words / strings of words that can strongly indicate democratic/republican origin.
    Build out model

Results: My best accuracy score was 0.73, part of the reason it was so low (particularly it wasnt too specific).  Ways I can improve the model in the future is by sampling it across a longer timespan (not just once) and balancing the classes. (currently the democratic subreddit is more active than the democratic).  In addition some more intuitive NLP work would be required, this was my first shot at using NLP in a project.  

Google Slides Presentation: https://docs.google.com/presentation/d/1IvY8T-RFcfHflcuTmkEGk8I_pl_8BJ0IiyhuCK_Dmvw/edit?usp=sharing

Project Directory:

Reddit_Webscraping: Used the PRAW (Python Reddit API Wrapper) to scrape data off the Reddit API

    Democrat_Reddit_Scrape-002.ipynb - Scraped the r/Democrats and saved it to a CSV
    Republican_Reddit_Scrape-001.ipynb - Scraped the r/Republicans and saved it to a CSV
    Republican.csv
    Democrats.csv

Cleaning_Aggregating_And_Seperating_Data:

    Political_Classifier_NLP_Cleaning_Aggregating_003-.ipynb Took both CSV's generated from the scrape and cleaned and aggreagated them for model building.
    
    comment_nlp.csv - Repulican and Democrat Subreddit post comments words
    replies_nlp.csv - Repulican and Democrat Subreddit post replies words
    title_nlp.csv - Repulican and Democrat Subreddit post title words
    data.csv - Repulican and Democrat Subreddit post numerical data
    Full_info.csv - Combined Rebpulican and Democrat data

Random Forest Models: Built models using the CSV's that were created in previous folder

    Random_Forest_Classifier_Comments.ipynb
    Random_Forest_Classifier_Numerical.ipynb
    Random_Forest_Classifier_Replies.ipynb
    Random_Forest_Classifier_Title.ipynb
    Random_Forest_Classifier_Combined_Dataset.ipynb
    


Thanks for reading, feel free to reach out anytime at gibert.medeiros8046@gmail.com for questions or comments, I would love any feedback as im constantly trying to expand my knowledge.
    