# final-project

***Sports Betting Machine Learning Project***

The goal of this project was to utilize a machine learning model that can predict the winner of an NBA game. 

The first step in this process was to scour the internet for a dataset that would provide us with rich historical NBA game data. Our team located several datasets on kaggle that provided us with overall game data, detailed player stats, and team rankings. 

The datasets can be found here: https://www.kaggle.com/nathanlauga/nba-games 

Once we imported the data files into pandas, we needed to decide which game statistics our model should focus on. After much discussion, we decided to focus on the field goal percentage, freethrow percentage, 3-pointer field goal percentage, total assists, and total rebounds for both the home and away teams. Once we had the dataset cleaned, we determined that the best feature to use to train our model would be the rolling average of all of the aforementioned statistical elements. 

With the rolling averages for the home and away team calculated, we used those features to train our four different models on game data spanning from 2004 to 2019, and then ran the test model on 2020 game data. The following models and their respective accuracies are listed below:

  - DecisionTreeClassifier 
    - 47% Accuracy
  - LogisticRegression 
    - 61% accuracy (Training)
    - 51% accuracy (Testing)
  - XGBoost
    - 51% Accuracy
  -RandomForestClassifier
    - 55% Accuracy

The RandomForestClassifier achieved the highest level of accuracy at 55%. 


