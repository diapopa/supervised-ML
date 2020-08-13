# supervised-ML

# Naive Random Oversampling
precision score: 
  High_risk: 0.01
  low_risk: 1.00
recall scores:
  High_risk: 0.64
  low_risk: 0.63
blanaced accuracy score: 0.636

# SMOTE Oversampling
precision score: 
  High_risk: 0.01
  low_risk: 1.00
recall scores:
  High_risk: 0.61
  low_risk: 0.68
blanaced accuracy score: 0.642

# Undersampling
precision score: 
  High_risk: 0.01
  low_risk: 1.00
recall scores:
  High_risk: 0.61
  low_risk: 0.42
blanaced accuracy score: 0.520

# Combination (Over and Under) Sampling
precision score: 
  High_risk: 0.01
  low_risk: 1.00
recall scores:
  High_risk: 0.72
  low_risk: 0.57
blanaced accuracy score: 0.647

The precision score looks at how many predicted instances are accuratly predicted. 
The precision scores for low_risk is 1.00 and for high_risk is 0.01 across tests because there are a high number of data points for low_risk and a low amount of data points for high_risk. 17118 and 97, respectively. This makes it easier to get accurate predictions for low risk instances since there are so many more instances.

The recall score is how likely the sampling method will correctly predict high risk or low risk.
The high risk recall scores apart from Combination sampling range in the low 0.60s and Combination sampling hit 0.72.
The low risk recall scores for both oversampling methods range in the 0.60s and Undesampling has a score 0.42 and Combination sampling has the lowest score of 0.57. 
These scores are overall low with Combination sampling having a higher score for high risk, meaning that it is 72% likely that the test will accurately predict that it is high risk.

The accuracy score compares the predicted and actual values to see how well the model performed.
All accuracy scores apart from Undersampling are around 64% with Undersampling having an accuracy score of 52%. These scores are a bit low and I would not recommend these models based on those scores.

# Final Recommendation
I would not use any of the models, because of the low precision for high risk and their overall lower recall and accuracy scores. My next step would be to scale the data to increase precision for high risk and re run the models.

