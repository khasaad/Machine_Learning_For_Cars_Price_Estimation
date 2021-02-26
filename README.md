
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
  <p>The best parameters  : {'n_estimators': 188, 'min_samples_split': 3, 'min_samples_leaf': 1, 'max_features': 'sqrt', 'max_depth': 18, 'bootstrap': False}</p>
  <ul>
    <li>r2 score test : 0.9635002634366892</li>
    <li>r2 score train : 0.990595627915352</li>
    <li>Kfold score mean : 93.6180174277052</li>
    <li>Kfold std deviation : 1.2996742902511158</li>
    <li>Kfold accuracy for each kfold : [0.94004127 0.93730947 0.91119167 0.94759439 0.94476407]</li>
    <li>Kfold variance : 0.00016891532607397417</li>
  </ul>
    <li>GridSearchCV</li>
  <p>The best parameters : {'bootstrap': False, 'max_depth': 18, 'max_features': 'sqrt', 'min_samples_leaf': 1, 'min_samples_split': 4, 'n_estimators': 177}</p>
  <ul>
    <li>r2 score test : 0.9637362114332027</li>
    <li>r2 score train : 0.9869405252800916</li>
    <li>Kfold score mean : 93.0294724497663</li>
    <li>Kfold std deviation : 9.173900139968046</li>
    <li>Kfold accuracy for each kfold : [0.84484988 0.68635042 0.85842274 0.6510353  0.66081528]</li>
    <li>Kfold variance : 0.008416044377810572</li>
  </ul>
  </ul>
</ul>

<h3>Feature Importance</h3>
<img src='https://user-images.githubusercontent.com/34131539/109364713-ad6a1880-788f-11eb-8ce6-f92a45c1b38f.PNG'>
