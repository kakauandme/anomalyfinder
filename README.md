# anomalyfinder - Science Hack Fest entry
A tool that finds anomalies in the data and plots them on the map to encourage further investigation for the causes of each anomaly


*anomaly_detection* - Reads a csv file of locations of the evens of interest with the relevant covariates 

*CSV to KML & JSON.ipynb* - converts longitude and latitude data to klm and json format for visualisation  

## Data preparation 
Matches observations from the data sources files and matches it with the event occurrence. The observation is considered relevant of it occurs within the specified radius from the location of event and within specified time interval 


## Demo
html prototype 

##anomaly detection fake data
testing the anomaly detection function on a artificially generated data




### Instalation

```
pip3 install virtualenv           # This may already be installed
virtualenv .env                   # Create a virtual environment
source .env/bin/activate          # Activate the virtual environment
pip3 install -r requirements.txt  # Install dependencies

jupyter notebook                  # Start iPython notebook

deactivate                        # Close session
```

