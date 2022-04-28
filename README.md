# Hyper-parameter-Optimization
Most models parameters are real-valued, and the
combinations of different parameters can be infinite.
Let’s look at the random forest model from scikit-learn:<br>

`RandomForestClassifier(
 n_estimators=100,
 criterion='gini',
 max_depth=None,
 min_samples_split=2,
 min_samples_leaf=1,
 min_weight_fraction_leaf=0.0,
 max_features='auto',
 max_leaf_nodes=None,
 min_impurity_decrease=0.0,
 min_impurity_split=None,
 bootstrap=True,
 oob_score=False,
 n_jobs=None,
 random_state=None,
 verbose=0,
 warm_start=False,
 class_weight=None,
 ccp_alpha=0.0,
 max_samples=None,
)`<br>

There are nineteen parameters, and all the combinations of all these parameters for
all the values they can assume are going to be infinite. Normally, we don’t have the
resource and time to do this. Thus, we specify a grid of parameters. A search over
this grid to find the best combination of parameters is known as **grid search**. 
