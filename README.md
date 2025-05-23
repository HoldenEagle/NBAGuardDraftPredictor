# NBAGuardDraftPredictor
This idea started as a final project idea for my Machine Learning class. Using NCAA college basketball box score and advanced stats from 2009-2021, I constructed two machine learning models. The first
model uses an XGBClassifier to predict whether an college point guard (Pure PGs and Scoring Point Guards) will get drafted that year in the NBA draft. Currently, this model is
at a stage where if it predicts a player will not get drafted, it is close to 99 percent accurate, and if it predicts a player will get drafted, it is 84 percent accurate. The next
model uses the XGBRegressor class with a logistic scale to predict where this college point guard will go in the draft pick wise. As there are 60 picks in the draft, so the logistic
model scales the prediction from 1-60, giving us a better predicter than a simple squared regression objective. On average, using RMSE (root mean square error) as our evaluation metric,
this model is only off about 7 picks. Even though this model is still a work in progress, it still performs very well on many of the picks, and still works as a good predicting model,
especially considering the fact that NBA teams need, and comparison to other players in their draft class. However, these two models could be influential to predicting where college
points guards go early on during the season, and could be of use to NBA agents, players, and sports bettors to evaluate and predict where players will end up in the NBA draft at the 
end of that season. In the testing set of the second model, some notable draft predictions include the following.


1. Toney Douglas : predicted pick 30.005742013454437 , actual pick 29.0
2. Dennis Smith, Jr. : predicted pick 8.376292377710342 , actual pick 9.0
3. Landry Shamet : predicted pick 28.292353361845016 , actual pick 26.0
4. Jawun Evans : predicted pick 39.8999325633049 , actual pick 39.0
5. Jalen Brunson : predicted pick 38.96916037797928 , actual pick 33.0
6. Malachi Flynn : predicted pick 28.371409952640533 , actual pick 29.0
7. Nolan Smith : predicted pick 25.8884516954422 , actual pick 21.0
8. Shake Milton : predicted pick 47.751150012016296 , actual pick 54.0

How to run these two model:
1. Clone this GitHub Repository
2. Run PreProcessing.ipynb to clean the dataset and create a new csv file that the two models use.
3. You can run either ipynb model and see results. You can also toy around to see if you can improve these models as well. Please
   share feedback if you can!

THIS REPOSITORY IS CURRENTLY BEING UPDATED TO INCLUDE COMBINE STATS AND PREDICTIONS FOR OTHER POSITIONS. 

Kaggle Dataset link:
https://www.kaggle.com/datasets/adityak2003/college-basketball-players-20092021
