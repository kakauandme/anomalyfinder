# Data preparation - Science Hack Fest entry

`hackfest_get_erai_data.ipynb` - function written by Peter Isaac that collects hourly meteorological data for the selected year. Data is saved as netcdf file with name being [year]_[longitude index]_[latitude index]
where longitude and latitude indices are calculated as following: 

fire["lon_index"] = int(((fire["longitude"]-longitude[0])/lon_resolution)+0.5)
fire["lat_index"] = int(((latitude[0]-fire["latitude"])/lat_resolution)+0.5)

where latitude[0] and longitude[0] are coordinates of the top left corner of the provided map.
 

`hackfest_get_data_from_netcdf.ipynb` - function written by Peter Isaac that takes a list of location in csv file and matches them to the meteorological data that is saved in netcdf files

`filter_data.ipynb` - selects fires with intensity over 50 and saves the locations to the csv file
We use fires with intensity over 50 in order to shrink our dataset and make it run faster


### Instalation

```
pip3 install virtualenv           # This may already be installed
virtualenv .env                   # Create a virtual environment
source .env/bin/activate          # Activate the virtual environment
pip3 install -r requirements.txt  # Install dependencies

jupyter notebook                  # Start iPython notebook

deactivate                        # Close session
```

