### project specification
 people order food on a online e-commerce platform. drivers take food from restaurant(placeId) to the customer (delivery city and delivery detail)

target: predicts the time from placing an order to order completation.
 ### approaches
 #### feature analysis and engineer
 - barplot, violinplot, boxplot for category vs numeric relation study
 - heatmap for category,category vs numeric relation study
 - kdeplot, histplot for distribution study
 - statistics by group by operation to give more detail information
 - openfe tool for more feature space searching 
 #### model study
 5 model were studied.
 model name | platform | score (rmse)
 -----------|----------|------------
 xgboost   | sklearn  |10.682, 10.60(by openfe augment)
lightgbm   | sklearn  |9.925
tabnet    | torch    |10.338
ft transformer| torch  |13.36
resnet    | tensorflow|10.23
#### end to end model
feature engineering by sklearn pipeline and end to end model was produced.
### conclusion
+ lightgbm is the best， tabnet and tesnet are also powerful
+ statistics by group by operation make a good performance improvement.
+ open fe tool make improvement to xgboost, but no improvement to other model.
+ pretraining have better performance on tabnet
+ ft transformer is not fit for such a problem


