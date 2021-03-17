# final-project

***Sports Betting Machine Learning Project***

  - Train algorithm on 2010-2018, then test on 2019. 
  - Run model on 32 games separately (Round 1), Run model on 16 games (Round 2), etc. - *ACCURACY SCORE*
  - Use XGboost
  - Clean data comes from Kaggle.
  - Once we have a model, predict a game from the day of or the night before.


The goal of this project was to utilize a machine learning model that can predict the winner of an NBA game. 

The first step in this process was to scour the internet for a dataset that would provide us with rich historical NBA game data. Our team located several datasets on kaggle that provided us with overall game data, detailed player stats, and team rankings. 

The datasets can be found here: https://www.kaggle.com/nathanlauga/nba-games 

Once we imported the data files into pandas, we needed to decide which game statistics our model should focus on. After much discussion, we decided to focus on the field goal percentage, freethrow percentage, 3-pointer field goal percentage, total assists, and total rebounds for both the home and away teams. Once we had the dataset cleaned, we determined that the best feature to use to train our model would be the rolling average of all of the aforementioned statistical elements. 

With the rolling averages for the home and away team calculated, we used those features to train our three different models on game data spanning from 2004 to 2019, and then ran the test model on 2020 game data. The following models and their respective accuracies are listed below:

  - LogisticRegression - 75.6% accuracy
  - 
