# Chevron_Market_Predictions_Final-Project
## Presentation link 

* [link to Presentation](https://docs.google.com/presentation/d/1x07APtx2-hP-XlsoJkWb0-fVOihlpX5NFsXfTRuWEKo/edit#slide=id.p)
## Topic 
 Chevron Corporation is an American multinational energy corporation. One of the successor companies of Standard Oil. I want to create a machine learning model to predict their closing prices for the next 30 days to see if Chevrons closing price will go up or down.
## Why 
I want to see if I can predict if Chevron continue to be a smart investment for investors using my knowledge of machine learning models.
## Source of data
I was able to get my stock data for Chevron from Yahoo Finance as a pip install. The pip install of yfinance had to be done in my anaconda prompt for my active environment created for the project. The yfinacne gives me the option of choosing a set period for the data or the entire history of the stock. I decided to use the data from 2010-01-04 to the present day.
## Questions I hope to answer
* Is chevron a smart invest?
* Why or why not?
* Other energy companies also a safe investment? 
## Explanations
* Data exploration phase; I was able to pull the data right from Yahoo Finance opposed to using a csv file. The Yahoo Finance has columns containing values for the date, the open of the stock dollar amount, high for the stock dollar amount, low for the stock dollar amount, close price for the stock dollar amount, dividends for the percentage of investment per individual investor, and stock splits the amount of shares multiplied by the split value per individual investor. 
* Analysis phase;  I decided the 'Dividends', 'Stock Splits', 'Low' ,’High', and date  columns were either empty or unneeded data for the machine learning model. No null values were found within the dataframe, after removing the ‘Dividends’ and ‘Stock Splits’ columns. Using the seaborn visualization tool I was able to look at relationships between my feature columns and target column using a hue for the target column of orange and blue and bar charts of red and blue. In the visualizations, the ‘Open’ and ‘Close’ columns show a strong linear regression over the years of the price going up but that is not what we are looking for in our model. In the bar chart of the counts of ‘Buy or Sell’ values, more of what we are looking for in our model, things seem very evenly distributed.  
## Machine Learning Model
* Description of preliminary data reprocessing. I reprocessed the data from the 'close' column only and used that to create a predicted column for an entire new column that will be used to train and test the data. The date column was reprocessed to include days and years to add to the dataframe.
* Description of preliminary feature engineering and preliminary feature selection, including decision making process. The 'close' column consits of the final price of the ticker symbol for each trading day which has been used to find if the stock was up in price from the open price showing a 1 for sell and a 0 for buy if the stock did not go up in price for the day. The date column was converted to create new columns to add features to my machine learning model. I choose the 'days', 'years', 'Open' and 'Volume' columns for my feature selection. 
* Description of how data was split into training and testing sets. Data was split into an 80/20 ratio, 80 % training on data and 20 % testing on data.
* Explaination of model choice, including limitations and benefits. I choose to go with a decision tree classifier and random forest classifier for models. I know I wanted to use a classifier for my model to get two target groups, a 'buy' group and a 'sell' group to see if Chevron stock was a good investment having more sell opportunity than buy. For the data I have it is limited, so having an unbalanced training and testing set can be bad for my models. 
## Dashboard
* Blue print for dashboard 
* * [link to Dashboard]()
* Story board on google slides
* Description of tools that will be used to create final dashboard
* tableau public 
* description of interactive element(s). 
** interactive chart of chevron stock, interactive chart of another energy stock. Charts do not show dollar amounts only sell or buy 0 or 1 for 0- 60 days.
