# Uber Data Analysis
Uber Data Analysis
This project aims at finding the factors driving the demand of Uber rides and also evaluate if the Uber drivers can earn reasonably (metric: hourly rate)  

# Installation
```
Install jupyter notebook (please see https://jupyter.org/install for the details)
```

# Required libraries
```
pip install pandas
pip install matplotlib
pip install seaborn
pip install geopandas
pip install folium
pip install mplcursors
pip install contextily
pip install shapely
pip install googlemaps
pip install pyspark
```
# Dataset
Since the dataset is too big to be uploaded to the Github, you can download it in the website -
https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page
file name - High Volume For-Hire Vehicle Trip Records (CSV)
time period: Jan - Jun 2020

# Run
```
git clone https://github.com/miki-lwy/Uber
cd Uber
pyspark
```

# Limitation of this project
Since the dataset does not include Uber drivers or users information, we cannot calculate the hourly rate with the corresponding ride details. Some people had uploaded their own Uber trip online. However, it is quite expensive to collect a reasonable amount of samples online. The alternatives would be calculating the hourly rate based on the estimated fare per ride for UberX and then taking the average value to get a general idea of the hourly rate. 
We also assume that the idling time of Uber cars should be excluded by this method.
