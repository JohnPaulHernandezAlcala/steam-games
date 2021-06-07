# Steam Games Analysis

<img src="https://www.slashgear.com/wp-content/uploads/2019/12/steamcure.jpg">


*Author: John Paul Hernandez Alcala*

## Description 
This project uses a data derived method for predicting which game would have above average ownership by Steam Users. A presentation that investigates which game features affect onwership count outcome and machine learning methods result in a model with either sensitivity(recall) 65% and specificity(precision) 76% or sensitivity 75% and specificity 72%.

## Where to Start First:

### 1. Access the [Importation_and_Cleaning_of_Data.ipynb](https://nbviewer.jupyter.org/github/JohnPaulHernandezAlcala/steam-games/blob/main/Importation_and_Cleaning_of_Data.ipynb) first and go from there.
### 2. Follow along with the coding narrative and comments.
### 3. Preview the uploaded presentation, [Steam Games Analysis](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Steam%20Games%20Analysis.pdf).

## From Analysis

### Top 10 Genre Combinations and Number of Genres
![](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/Top10Genres.png)
![](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/NumOfGenresBar.png)

### Top 10 TopTag and Number of Tags
![](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/Top10Tags.png)
![](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/NumOfTagsBar.png)

## Model in Action
Below, we can see the prediction ability in action from both the original model and the model with a custom threshold

### Original Model
![Actual Answer Vs Model Prediction Price](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/FinalModelinAction.png)

### Model with Custom Threshold
![](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/FinalModelwThresholdinAction.png)

### Model with Custom Threshold Confusion Matrix
![Confusion Matrix](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/FinalModelConMatThres.png)

Here we see our model with and without a threshold implemented. This threshold makes our model more sensitive, but less specific or precise than the default model; that is, our threshold model allows for more false positives in order to reduce false negatives. With the threshold model, we are able to predict ~65% of games as having above average owners count or ownership, and it also predicted 76% of games as not above average when they were indeed not above. This is compared to our original model that was able to predict 75% of games as above average when they were indeed above and 72% of clients as games not above average when they were actually not.

### ROC-AUC Graph of 5 Models with Custom Threshold
![](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/FinalModelROC-AUC.png)

From this model, we can conclude that our top features are the following: 

### Top 10 Features
![Top 10 Features](https://github.com/JohnPaulHernandezAlcala/steam-games/blob/main/Images/Top10FeaturesfromFinalModel.png)

## Conclusion
From the analysis of this data and implemenation of multiple models and thresholds, it was determined that the best model from the 5 used models in this project is the random forest model with a threshold of 0.40 because of its highest recall or sensitive score of 0.71 for 'yes', specificity or precision of 65%, and AUC of 0.78


* Number of Tags 
* Number of Languages
* Does Not Have YouTube Views
* Number of Categories,
* Price 
* Has YouTube Views
* Had peak concurrent players yesterday
* Does Have an Old userscore
* Does Not Have an Old userscore
* Top Voted Tag as Indie

With this model and our total analysis, we can produce three business recommendations:

* Have more than 6 tags for your game
* Make sure you get game content published on YouTube
* Make a game that has the only genre as action or action, adventure combination

## Support
If you need any help, please email me at johnhdz1023@gmail.com.

## Acknowledgments
[Steam](https://store.steampowered.com/)
[SteamSpy](https://steamspy.com/)

I want to thank my girlfriend, Haley, [Flatiron School](https://flatironschool.com/), my cohort, and my technical advisor, Lindsey Berlin, and [Eli](http://linkedin.com/in/jacob-eli-thomas-4377037).

## Contribution
See [CONTRIBUTING.md](https://github.com/JohnPaulHernandezAlcala/House_Sale_Prices/blob/master/CONTRIBUTING.md)

# License
See [LICENSE.md](https://github.com/JohnPaulHernandezAlcala/House_Sale_Prices/blob/master/LICENSE.md)

# Image Sources:
https://www.slashgear.com/wp-content/uploads/2019/12/steamcure.jpg


#### -- Project Status: [Completed]
# steam-games
