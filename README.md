# Bank Targeted Marketing

<img src="https://cdn.wallethub.com/wallethub/posts/76002/banking-landscape-report.png" width="300"><img src="https://img2.pngio.com/business-growth-chart-png-transparent-growth-charts-transparent-business-growth-png-820_387.png" width="500">

<img src="https://acrobatant.com/wp-content/uploads/2018/09/Target_Marketing.jpg" width="600">

*Author: John Paul Hernandez Alcala*

## Description 
This project uses a data derived method for predicting which client type should be targeted for successful bank telemarketing. A presentation that investigates which client features affect marketing success rate and machine learning methods result in a mode with good sensitivity (~73%) and good specificity (~73%).



## Where to Start First:

### 1. Access the [Preprocessing.ipynb](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Preprocessing.ipynb) first and go from there or look at all the code at once in [Total_Code.ipynb](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Total_Code.ipynb).
### 2. Follow along with the coding narrative and comments.
### 3. Preview the uploaded presentation, [Bank Targeted Marketing](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Bank%20Targeted%20Marketing.pdf).

## From Analysis

### Job-Education Pair Graph
![](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Education_Job__prop_Graph.png)
![](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Education_Job_Graph.png)

### Job-Education Pair Age Distribution
![](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/AgeDistribution.png)

### Month Contacted and Times Contacted Before Marketing Campaign
![](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Month_Previous_Graph.png)

## Model in Action
Below, we can see the prediction ability in action from both the original model and the model with a custom threshold

### Original Model
![Actual Answer Vs Model Prediction Price](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Model_in_Action.png)

### Model with Custom Threshold
![](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Model_in_Action_with_threshold.png)

### Model with Custom Threshold Confusion Matrix
![Confusion Matrix](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/RF_ConfusionMatrix_with_Threshold.png)

Here we see our model with and without a threshold implemented. This threshold makes our model more sensitive, but less specific and precise than the default model; that is, our threshold model allows for more false positives in order to reduce false negatives which is our goal in this scenario. With the threshold model, we are able to predict ~72% of clients as subscribers who were indeed subscribers, and it also predicted 73% of clients as non-subscribers who were indeed not subscribers. This is compared to our original model that was able to predict 56% of clients as subscribers who were indeed subscribers and 92% of clients as non-subscribers who were indeed not subscribers.

### ROC-AUC Graph of 5 Models with Custom Threshold
![](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/ROC-AUC_with_threshold_Graph.png)

From this model, we can conclude that our top features are the following: 

### Top 10 Features
![Top 10 Features](https://github.com/JohnPaulHernandezAlcala/Bank-Targeted-Marketing/blob/master/Top10Features_clear.png)

## Conclusion
From the analysis of this data and implemenation of multiple models and thresholds, it was determined that the best model from the 5 used models in this project is the random forest model with a threshold of 0.2701844 because of its highest recall score of 0.72 for 'yes', AUC of 0.79, specificity of ~72%, and sensitivity of ~72%. 

## Recommendations from Model and Analysis:
Subscriber outcome is high for:
* Top Ten Features of Model
* Students who have an education level at 'basic.4y', 'basic.9y', 'high.school'
* Certain age ranges for students, retired, and unemployed
* Client contact efforts and timing: month contact, and previous calls


## Support
If you need any help, please email me at johnhdz1023@gmail.com.

## Acknowledgments
[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014

I want to thank my girlfriend, Haley, [Flatiron School](https://flatironschool.com/), my cohort, and my technical advisor, [Eli](http://linkedin.com/in/jacob-eli-thomas-4377037), for input on this project. I wish he could have seen the end product.

## Contribution
See [CONTRIBUTING.md](https://github.com/JohnPaulHernandezAlcala/House_Sale_Prices/blob/master/CONTRIBUTING.md)

# License
See [LICENSE.md](https://github.com/JohnPaulHernandezAlcala/House_Sale_Prices/blob/master/LICENSE.md)

# Relevant Papers:

[S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014](http://media.salford-systems.com/video/tutorial/2015/targeted_marketing.pdf)

[S. Moro, R. Laureano and P. Cortez. Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimaraes, Portugal, October, 2011. EUROSIS. [bank.zip]](https://www.semanticscholar.org/paper/Using-data-mining-for-bank-direct-marketing%3A-an-of-Moro-Laureano/a175aeb08734fd669beaffd3d185a424a6f03b84)

# Image Sources:
https://cdn.wallethub.com/wallethub/posts/76002/banking-landscape-report.png

https://img2.pngio.com/business-growth-chart-png-transparent-growth-charts-transparent-business-growth-png-820_387.png

https://acrobatant.com/wp-content/uploads/2018/09/Target_Marketing.jpg

#### -- Project Status: [Completed]
# steam-games
