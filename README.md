# Chevron_Market_Predictions_Final-Project
## Presentation link 

* [link to Presentation](https://docs.google.com/presentation/d/1x07APtx2-hP-XlsoJkWb0-fVOihlpX5NFsXfTRuWEKo/edit#slide=id.p)
## Topic 
 Chevron Corporation is an American multinational energy corporation. One of the successor companies of Standard Oil. I want to create a machine learning model to predict their closing prices for the next 30 days to see if Chevrons closing price will go up or down.
## Why 
Can Chevron continue to be a safe and wise investment for investors?  
## Source of data
I was able to get my stock data for Chevron from Yahoo Finance as a pip install. The pip install of yfinance had to be done in my anaconda prompt for my active environment created for the project. The yfinacne gives me the option of choosing a set period for the data or the entire history of the stock. I decided to use the data from 2020-01-01 to the present day.
## Questions I hope to answer
* Is chevron a safe invest?
* Why or why not?
* Other energy companies also a safe investment? 
## Explanations
* Data exploration phase was more challenging than I anticipated. I was able to find downloadable cvs files for Chevron stock in kaggle.com, yahoo, and other major search engine sites however download and reading the cvs files into my jupyter notebook required me to change data types from objects into integers or floats inorder to manipulate the data for a machine learning model. However using the yfinance package allowed me to read the data from yahoo and not change any of the data types. This will save me time and some lines of code in the long run.
* Analysis phase for this challenge has taken the most time to try different models to see which will be most accurate.
## Machine Learning Model
* Description of preliminary data reprocessing. I reprocessed the data into the 'close' column only and used that to create a predicted column for an entire new data set that will be used to train and test the data. The 'close' column consits of the final price of the ticker symbol for each trading day, in my case Chevron, CVX.
* Description of preliminary feature engineering and preliminary feature selection, including decision making process
* Description of how data was split into training and testing sets. Data was split into an 80/20 ratio, 80 % training od data and 20 % testing on data.
* Explaination of model choice, including limitations and benefits
## Dashboard
* Blue print for dashboard 
* Story board on google slides
* Description of tools that will be used to create final dashboard
* description of interactive element(s)
