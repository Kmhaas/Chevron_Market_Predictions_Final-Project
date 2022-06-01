# Chevron_Market_Predictions_Final-Project
## Presentation link 

* [link to Presentation](https://docs.google.com/presentation/d/1x07APtx2-hP-XlsoJkWb0-fVOihlpX5NFsXfTRuWEKo/edit?usp=sharing)
## Topic 
Chevron Corporation is an American multinational energy corporation. One of the successor companies of Standard Oil. I want to create a machine learning model to classify each trading day as a ‘Buy’ or ‘Sell’ opportunity. I want to see if I can predict if Chevron continue to be a smart investment for investors using my knowledge of machine learning models.
## Source of data
I was able to get my stock data for Chevron from Yahoo Finance as a csv file. The Yahoo Finance page gives me the option of choosing a set period for the data or the entire history of the stock. I decided to use the data from 2010-01-04 to the present day.
## Questions I hope to answer
* Is chevron a smart invest?
* Is there more ‘Sell’ or ‘Buy’ opportunity for chevron stock today ?

## Explanations
* Data exploration phase; I only found the data from yahoo finance as relevant. Other models use columns created drawing conclusions from other factors to create more data for stock predictions. The raw data from the market was all I used, the ‘open’,’close’,volume’ and ‘date’. I dropped the ‘adj close’,’low’ and ‘high’ columns.
*  Analysis phase;  I decided the 'Adj Close', 'Low' ,and ’High', columns were unneeded data for the machine learning model. No null values were found within the dataframe. Using the seaborn visualization tool I was able to look at relationships between my feature columns and target column using a hue for the target column of orange and blue and bar charts of red and blue. In the visualizations, the ‘Open’ and ‘Close’ columns show a strong linear regression over the years of the price going up but that is not what we are looking for in our model. In the bar chart of the counts of ‘Buy or Sell’ values, more of what we are looking for in our model, things seem very evenly distributed for the counts of ‘buy’ and ‘sell’ opportunities.
 
## Machine Learning Model
* Description of preliminary data reprocessing; I re-processed the data from the 'close' column to create my target data. The date column was convert to a pandas datetime and reprocessed to include new column, ‘days’, to add to the dataframe.
* Description of how data was split into training and testing sets; Data was split into an 80/20 ratio, 80 % training on data and 20 % testing on data. I can see I have 2495 values for a training set and 624 for a testing set. I scaled the data for a standardscaler instance for my neural network. The  data I have is limited so having an unbalanced training and testing could be bad for my models. So far I have trained the model by splitting it from the entire data set, scaling the data and additional training will take place during the neural network model using the x_train_scaled data for fitting.
* Description of preliminary feature engineering and preliminary feature selection, including decision making process; The 'close' column consists of the final price of the ticker symbol for each trading day which has been used to find if the stock was up in price from the open price showing a 1 for sell and a 0 for buy if the stock did not go up in price for the day. The date column was converted to create new columns to add features to my machine learning model. I choose the 'days', 'years', 'Open' and 'Volume' columns for my feature selection
* Explanation of model choice; Including limitations and benefits. I know I wanted to use a classifier for my model to get two target groups, 'buy' and 'sell' .  I choose to try a decision tree classifier and random forest classifier for models. To begin with. Both models performed about the same so I tried a deep neural network and increased my accuracy. I decided to use that one for my final model.
* Explanation of changes in model, After deciding the neural network model would be the most accurate, I created four neural network models. I found the second one was the most accurate. The second neural network has only two hidden layers and all three activation functions are different. The first activation function was ‘sigmoid’,then ‘relu’, and the output function was ‘tanh’. The third and fourth models had both more hidden layers and repeated activation functions. I wanted to try more layers to see if that would increase accuracy, it did not. I then wanted to change the activation functions using some repeatedly still it did not increase my accuracy resulting in the second model being the most accurate.


## Dashboard

*  [link to Dashboard](https://public.tableau.com/app/profile/kevin7960/viz/CVX_Dash1/Interactive#2)







## Speaker notes per Presentation
Slide 2:
Chevron Corporation is an American multinational energy corporation. One of the successor companies of Standard Oil. I want to create a machine learning model to classify each trading day as a ‘Buy’ or ‘Sell’ opportunity. I want to see if I can predict if Chevron continue to be a smart investment for investors using my knowledge of machine learning models.
Slide 3:
I was able to get my stock data for Chevron from Yahoo Finance as a csv file. The Yahoo Finance page gives me the option of choosing a set period for the data or the entire history of the stock. I decided to use the data from 2010-01-04 to the present day.
Slide 5: 
I only found the data from yahoo finance as relevant. Other models use columns created drawing conclusions from other factors to create more data for stock predictions. The raw data from the market was all I used, the ‘open’,’close’,volume’ and ‘date’.
Slide 6: 
Analysis phase;  I decided the 'Adj Close', 'Low' ,and ’High', columns were unneeded data for the machine learning model. No null values were found within the dataframe.
Slide 7: 
Using the seaborn visualization tool I was able to look at relationships between my feature columns and target column using a hue for the target column of orange and blue and bar charts of red and blue. In the visualizations, the ‘Open’ and ‘Close’ columns show a strong linear regression over the years of the price going up but that is not what we are looking for in our model.
Slide 8:
In the bar chart of the counts of ‘Buy or Sell’ values, more of what we are looking for in our model, things seem very evenly distributed for the counts of ‘buy’ and ‘sell’ opportunities.
Slide 9:
Description of preliminary data reprocessing; I re-processed the data from the 'close' column to create my target data. The date column was convert to a pandas datetime and reprocessed to include new column, ‘days’, to add to the dataframe.
Slide 10:
Description of how data was split into training and testing sets; Data was split into an 80/20 ratio, 80 % training on data and 20 % testing on data. I can see I have 2495 values for a training set and 624 for a testing set. I scaled the data for a standardscaler instance for my neural network. So far I have trained the model by splitting it from the entire data set, scaling the data and additional training will take place during the neural network model using the x_train_scaled data for fitting.
Slide 11:
Description of preliminary feature engineering and preliminary feature selection, including decision making process; The 'close' column consists of the final price of the ticker symbol for each trading day which has been used to find if the stock was up in price from the open price showing a 1 for sell and a 0 for buy if the stock did not go up in price for the day. The date column was converted to create new columns to add features to my machine learning model. I choose the 'days', 'years', 'Open' and 'Volume' columns for my feature selection
Slide 12:
Explanation of model choice; Including limitations and benefits. I know I wanted to use a classifier for my model to get two target groups, 'buy' and 'sell'.  I choose to try a decision tree classifier and random forest classifier for models. To begin with. Both models performed about the same, so I tried a deep neural network and increased my accuracy. I decided to use that one for my final model.
Slide 19:
Explanation of changes in model, After deciding the neural network model would be the most accurate, I created four neural network models. I found the second one was the most accurate. The second neural network has only two hidden layers and all three activation functions are different. The first activation function was ‘sigmoid’, then ‘relu’, and the output function was ‘tanh’. The third and fourth models had both more hidden layers and repeated activation functions. I wanted to try more layers to see if that would increase accuracy, it did not. I then wanted to change the activation functions using some repeatedly still it did not increase my accuracy resulting in the second model being the most accurate.
Slide 20:
The highest accuracy score I have been able to produce is 54.48 %.

Slide 21:

141 TN  
139 FN 
167 FP 
177 TP
Precision Score: 0.5145
Recall Score: 0.5601
F1 Score: 0.5363 
Slide 22:
All code has been written in the python language in a jupyter notebook or visual studio code notebook. A new visualization tool I used for this project was seaborn, an import tool used to create visual graphs for the data. Tableau was also used to create an interactive dashboard.
Slide 24:
According to the model the Chevron stock has more sell opportunity. History has shown a continuous trend of Chevron stock increasing in price even with slight dips over the years.




