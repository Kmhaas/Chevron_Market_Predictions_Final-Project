# Chevron_Market_Predictions_Final-Project
## Presentation link 

* [link to Presentation](https://docs.google.com/presentation/d/1x07APtx2-hP-XlsoJkWb0-fVOihlpX5NFsXfTRuWEKo/edit#slide=id.p)
## Topic 
 Chevron Corporation is an American multinational energy corporation. One of the successor companies of Standard Oil. I want to create a machine learning model to predict their closing prices for the next 30 days to see if Chevrons closing price will go up or down.
## Why 
Can Chevron continue to be a safe and wise investment for investors?  
## Source of data
I was able to get my stock data for Chevron from Yahoo Finance as a pip install. The pip install of yfinance had to be done in my anaconda prompt for my active environment created for the project. The yfinacne gives me the option of choosing a set period for the data or the entire history of the stock. I decided to use the data from 2010-01-01 to the present day.
## Questions I hope to answer
* Is chevron a safe invest?
* Why or why not?
* Other energy companies also a safe investment? 
## Explanations
* Data exploration phase was more challenging than I anticipated. I was able to find downloadable csv files for Chevron stock in kaggle.com, yahoo, and other major search engine sites, instead I was able to pull the data right from Yahoo Finance opposed to a csv file. I decided the 'Dividends', 'Stock Splits', 'Low' and ‘'High' columns were unneeded data for the machine learning model and the Dividends and Stock Splits only apply to the dollar amount invested by the investor resulting in all of these columns being dropped from the data frame. The remaining columns are used as my features, ‘days', 'years', ‘Open’, and ‘Volume’ columns. I created a target column for the machine learning of ‘Buy_Sell’ 0 and 1 for the classification from using the ‘Close’ column for each day. I used seaborn to visualize any relationships between my feature data. 
* Analysis phase I went with a decision tree classifier for my model. I also intended on using a random forest classifier for the model as well to see which will be the most accurate. In both models I have overfitted my results. I will have to tune both models to see if I can improve my accuracy results. I will have to look at my features, add more, get synthetic data or change my target parameters. 
## Machine Learning Model
* Description of preliminary data reprocessing. I reprocessed the data from the 'close' column only and used that to create a predicted column for an entire new column that will be used to train and test the data. The date column was reprocessed to include days and years to add to the dataframe.
* Description of preliminary feature engineering and preliminary feature selection, including decision making process. The 'close' column consits of the final price of the ticker symbol for each trading day which has been used to find if the stock was up in price from the open price showing a 1 for sell and a 0 for buy if the stock did not go up in price for the day. The date column was converted to create new columns to add features to my machine learning model. I choose the 'days', 'years', 'Open' and 'Volume' columns for my feature selection. 
* Description of how data was split into training and testing sets. Data was split into an 80/20 ratio, 80 % training on data and 20 % testing on data.
* Explaination of model choice, including limitations and benefits. I choose to go with a decision tree classifier and random forest classifier for models. I know I wanted to use a classifier for my model to get two target groups, a 'buy' group and a 'sell' group to see if Chevron stock was a good investment having more sell opportunity than buy. For the data I have it is limited so having an unbalanced training and testing set has shown issues with my accuracy overall with my models. 
## Dashboard
* Blue print for dashboard 
* Story board on google slides
* Description of tools that will be used to create final dashboard
* description of interactive element(s). 
** interactive chart of chevron stock, interactive chart of another energy stock. Charts do not show dollar amounts only sell or buy 0 or 1 for 0- 60 days.
