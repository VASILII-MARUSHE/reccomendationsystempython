# Recommendation systems for book shop
## Data preprocessing and choice of the most relevant of them:
1.	First, we should narrow down the area of our clients. We assume that our recommendation will item-user approach (based on task).  So we take all users that rate the certain book and any other books that these users rated. 
2.	Using cluster analysis, we can in theory reduce the search area by choosing one of the biggest clusters for example or we can come up with better criteria for choosing more relevant segment which we will work on. 
## Recommendation based on cosine similarity:
1.	Advantages of this recommendation system:
1.1	Discovering new products. If a group of users gives high ratings to certain products, the collaborative filtering system can recommend them to a user who exhibits similar behavior but has not yet seen these products.
1.2	No need for specialized knowledge. The method requires only data on user behavior.
1.3	This measure easy to interpret 

2.	Disadvantages of collaborative filtering
2.1	If no users have rated the content, no recommendations will be made.will not be given
2.2	users who do not have overlapping tastes with other users will not receive good recommendations.
2.3	This method based on assumption of familiarity of users. So if it is not we can not consider that if one user have a familiar taste with other by our data. It doesn’t mean that user1 and user2 will have the same taste on something else. 
2.4	Bad working when we have a lot of 0 in our rating matrix.
 
## ALS (Alternative Least Square) a bmi recommendation 
1.	Pluses of model 
1.1	Works well with sparse user-item data.
1.2	 Handles implicit feedback (e.g., clicks, purchases) better than standard CF models.
1.3	Scales efficiently for large datasets with millions of interactions.
1.4	Unlike the previous method, this method provides a variety of recommendations in different domains. The method adapts to users' preferences and interests
1.5	the quality of recommendations directly depends on user ratings
2.	Cons of models: 
2.1	Cold start 
2.2	Black sheep
## Evaluation of ALS. 
1.	MAE, Precision,@10 NPCG@10
