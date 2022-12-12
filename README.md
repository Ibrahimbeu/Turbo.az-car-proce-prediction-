# Turbo.az-car-price-prediction
## Prepearing dataset for model. Here we have messy data (include some missing values, outliers). Also we need to get some intuition about data. That's why I apply some visualization
## In part2 I create optimizer class which includes all preprocessing and model building parts in one class. It includes __init__ instructos, prep(for preprocessing), hyp_optimizer (which is alternative to GridSearchCV),fit, predict and etc.
## At the end we get:
                      param_space={"max_depth":[2,4,6],"min_samples_split":[4,6,8],'max_features':['sqrt', 'log2']}
                      op= optimizer(DecisionTreeRegressor,param_space,fold=4,tuning='binary_search')
                      op.fit(df)
