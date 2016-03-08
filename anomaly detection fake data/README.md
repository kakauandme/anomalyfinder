# anomalyfinder

Testing anomaly detection algorithm on the fake(artificially generated) data while the real data is being pulled.

 

`fake_data_generation.ipynb` - generates a  fakedata.csv file with columns names: longitude, latitude, datetime, X1, X2, X3. The last 3 column are imitating real covariate data


`anomaly_detection_demo.ipynb` - runs anomaly detection algorithm, plots the outliers and returns website_data.js with json data that contains original data + outlier flag  