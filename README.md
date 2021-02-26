
# Machine_Learning_For_Cars_Price_Estimation

<p> Using :</p> KFold cross validation and RandomForestRegressor as ML model with RandomisedSearchCV and GridSearchCV.

<ul>
  <li>KFold and cross validation</li>
  <li>RandomForestRegressor</li>
  n_estimators = [int(x) for x in np.linspace(start=100, stop=200, num=10)] </br>
  max_features = [None, 'auto', 'sqrt']</br>
  max_depth = [10, 14, 18]</br>
  min_samples_split = [2, 3, 4]</br>
  min_samples_leaf = [1, 2]</br>
  bootstrap = [True, False]</br>

param_grid = {'n_estimators': n_estimators,
'max_features': max_features,
'max_depth': max_depth,
'min_samples_split': min_samples_split,
'min_samples_leaf': min_samples_leaf,
'bootstrap': bootstrap}

  <ul>
    <li>RandomisedSearchCV</li>
  <p>{'n_estimators': [100, 111, 122, 133, 144, 155, 166, 177, 188, 200], 'max_features': [None, 'auto', 'sqrt'], 'max_depth': [14, 18], 'min_samples_split': [2, 3, 4], 'min_samples_leaf': [1, 2], 'bootstrap': [True, False]}
</p>
    <li>GridSearchCV</li>
  </ul>
</ul>

<h3>Feature Importance</h3>
<img src='https://user-images.githubusercontent.com/34131539/109364713-ad6a1880-788f-11eb-8ce6-f92a45c1b38f.PNG'>
