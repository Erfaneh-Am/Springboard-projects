# Take Home Challenge - Relax Inc. 

The dataset comprised information on users and their engagement data for 8,823 users, out of which 1,602 were identified as "adopted users". The primary focus of my investigation was to determine the key factors influencing user adoption. Through analysis, I discovered that the length of usage emerged as the most important factor. Length of usage was defined as the duration between account creation and the latest session. 
During the analysis of feature correlation, a heat map was generated and strong correlation was observed between adopted users and the "duration_usage" feature. The second correlated feature was "visited" which is the number of the times the user visited the product since the creation of the account. 

## Feature Correlation Heatmap
![0AD0AB94-E9E5-4D95-85BE-E9F409F24279](https://github.com/Erfaneh-Am/Springboard-projects/assets/121911081/f3dc720c-31ba-4771-86b0-3f84c784f68a)


Next, a Random Forest Classifier model was trained on the data and tuned ('criterion': 'entropy', 'max_depth': 5), which was able predict the "adopted_user" feature with more than 98% accuracy. Through the use of the "feature_importance" attribute of the Random Forest classifier, we verified that the duration of usage and the frequency of user visits to the product were the two most significant factors influencing user adoption with latter to be the most important feature. 

## Best Random Forest Feature Importance
![0069B3D2-D266-47E7-AE64-BAEA4C01B1C5_1_201_a](https://github.com/Erfaneh-Am/Springboard-projects/assets/121911081/03e892b6-a253-4f82-9064-0df5a1fe8679)
