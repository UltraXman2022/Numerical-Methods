<h1>Project description</h1>
Rusty Bargain used car sales service is developing an app to attract new customers. In that app, you can quickly find out the market value of your car. You have access to historical data: technical specifications, trim versions, and prices. You need to build the model to determine the value.

<h2>Rusty Bargain is interested in:</h2>
<ul><li>the quality of the prediction</li>
<li>the speed of the prediction</li>
<li>the time required for training</ul></li>

<h2>Project instructions</h2>
<ol><li>Download and look at the data</li>
<li>Train different models with various hyperparameters (You should make at least two different models, but more is better. Remember, various implementations of gradient boosting don't count as different models.) The main point of this step is to compare gradient boosting methods with random forest, decision tree, and linear regression.</li>
<li>Analyze the speed and quality of the models/ol></li>

<h2>Notes:</h2>
<ul><li>Use the RMSE metric to evaluate the models</li>
<li>Linear regression is not very good for hyperparameter tuning, but it is perfect for doing a sanity check of other methods. If gradient boosting performs worse than linear regression, something definitely went wrong</li>
<li>On your own, work with the LightGBM library and use its tools to build gradient boosting models</li>
<li>Ideally, your project should include linear regression for a sanity check, a tree-based algorithm with hyperparameter tuning (preferably, random forrest), LightGBM with hyperparameter tuning (try a couple of sets), and CatBoost and XGBoost with hyperparameter tuning (optional)</li>
<li>Take note of the encoding of categorical features for simple algorithms. LightGBM and CatBoost have their implementation, but XGBoost requires OHE</li>
<li>You can use a special command to find the cell code runtime in Jupyter Notebook. Find that command</li>
<li>Since the training of a gradient boosting model can take a long time, change only a few model parameters</li>
<li>If Jupyter Notebook stops working, delete the excessive variables by using the del operator:</ul></li>

  del features_train
   
<h2>Data description</h2>
The dataset is stored in file /datasets/car_data.csv. download dataset.

<h3>Features</h3>
<ul><li>DateCrawled — date profile was downloaded from the database</li>
<li>VehicleType — vehicle body type</li>
<li>RegistrationYear — vehicle registration year</li>
<li>Gearbox — gearbox type</li>
<li>Power — power (hp)</li>
<li>Model — vehicle model</li>
<li>Mileage — mileage (measured in km due to dataset's regional specifics)</li>
<li>RegistrationMonth — vehicle registration month</li>
<li>FuelType — fuel type</li>
<li>Brand — vehicle brand</li>
<li>NotRepaired — vehicle repaired or not</li>
<li>DateCreated — date of profile creation</li>
<li>NumberOfPictures — number of vehicle pictures</li>
<li>PostalCode — postal code of profile owner (user)</li>
<li>LastSeen — date of the last activity of the user</ul></li>

<h3>Target</h3>
<ul><li>Price — price (Euro)</ul></li>
