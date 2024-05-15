# MLP-project-Last-term
<p>This is last-term machine learning project. it is in form of  a Kaggle competition held between IITM students.</p>

<p><b>Situation:</b></p>
<p>Somato company want to predict the rating of a recipe from the comments of users.</p>

<p><b>Task:</b></p>
Build models that can guess the ratings for each recipe using this information.

<p><b>Data set descriptions:</b></p>
<p>1. RecipeNumber: Placement of the recipe on the top 100 recipes list.</p>
<p>2. RecipeCode: Unique ID of the recipe used by the site.</p>
<p>3. RecipeName: Name of the recipe the comment was posted on.</p>
<p>4. CommentID: Unique ID of the comment.</p>
<p>5.UserID: Unique ID of the user who left the comment.</p>
<p>6. Username: Name of the user.</p>
<p>7. UserReputation: Internal score of the site, roughly quantifying the past behaviour of the user.</p>
<p>8. CreationTimestamp: Time at which the comment was posted as a Unix timestamp.</p>
<p>9. ReplyCount: Number of replies to the comment.</p>
<p>10. ThumbsUpCount: Number of up-votes the comment has received.</p>
<p>11. ThumbsDownCount: Number of down-votes the comment has received.</p>
<p>12. Rating: The score on a 1 to 5 scale that the user gave to the recipe. A score of 0 means that no score was given (Target Variable).</p>
<p>13. BestScore: Score of the comment, likely used by the site to help determine the order comments appear in.</p>
<p>14. Recipe_Review: The text content of the comment.</p>

<p><b>Action:</b></p>

<p>1. Observe the data and write down your data summary.</p>
<p>2. Import all necessary libraries and perform EDA.</p>
<p>3.Split features and target variables from training data.</p>
<p>4.Perform feature engineering.</p>
<p>5. Apply one-hot encoder on categorical and standard scaler on numerical data.</p>
<p>6. Perform TFID-vectorization on a recipe-review column to clean text.</p>
<p>7. Build the baseline model.</p>
<p>8. Applied logistics regression and performed hyperparameter tuning with randomized search CV.</p>
<p>9. Applied KNN algorithm and performed hyperparameter tuning with randomized search CV.</p>
<p>10. Applied random forest algorithm and performed hyperparameter tuning with randomized search CV.</p>
<p>11. Applied Lightboost classifier algorithm and performed hyperparameter tuning with randomized search CV.</p>
<p>12. Applied XGboost algorithm and performed hyperparameter tuning with randomized search CV.</p>
<p>13. Applied bagging classifier algorithm and performed hyperparameter tuning with randomized search CV.</p>
<p>14. Applied stacking algorithm and performed hyperparameter tuning with randomized search CV.</p>
<p>15. perform the same steps in test data.</p>
<p>16. train model with best accuracy model.</p>

<p><b>Result:</b></p>
<p>1. Stacking classifier, XGBoost, and LightGBM are the best-performing models.</p>
<p>2. Best hyperparameter for the Light GBM classifier are:    {num_leaves=40,min_child_samples=30,max_depth=15,learning_rate=0.1,feature_fraction=0.9,bagging_fraction=1}</p>
<p>3. The best Hyperparameters for the Random Forest classifier are:{'n_estimators': 100, min_samples_split': 6, 'max_features': 'sqrt', 'bootstrap': False}</p>
<p>4. Best Hyper parameter for Bagging classifier are :{'n_estimators': 500, max_samples=100, 'max_features': 100, 'bootstrap': False}</p>
<p>5. The best accuracy score achieved is 0.80004</p>
