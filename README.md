# NYC CitiBike
Module 15 Challenge - Data Visuauzation using Tableau

## Resources
Operating Platform: Windows 11 Pro [Buy Windows 11 Pro](https://www.microsoft.com/en-us/d/windows-11-pro/dg7gmgf0d8h4?rtc=1) Build 22621</br>
IDE Software: [Tableau Desktop](https://www.tableau.com/products/desktop/download) Build 2022.3.1 (20223.22.11.08.0821) 64-bit</br>
Source Data: [Historical 201908-citibike-tripdata](https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip)
Resource files: ADD COMPLETED SCRIPT HERE
Program Languages: Jupyter Notebook [Install](https://jupyter.org/install)
Jupyter Packages: [Pandas](https://pandas.pydata.org/), [datetime](https://pandas.pydata.org/docs/user_guide/timeseries.html)

## Overview
Using historical data from a bikeshare company in NYC and their historical data, it will be used as a data sample to build a few visualazations using Tableau to help convience a fictious investors in Des Moines, Iowa that creating their own BikeSharing company is a good idea. Using Tableau the following will be created to display: 
* The length of time that bikes are checked out for all riders and genders.
* The number of bike trips for all riders and genders for each hour of each day of the week.
* The number of bike trips for each type of user and gender for each day of the week.

## Deliverable 1: Change Trip Duration to a Datetime Format
Using Jupyter notebook the dataset is imported from a CSV file into a dataframe. The dataframe is then validated the information was imported correctly then using the below script the specific column is switched from int64 to datatime64. 
```
# 3. Convert the 'tripduration' column to datetime datatype.
citibike_df['tripduration'] = pd.to_datetime(citibike_df['tripduration'], unit='s')
```
The cleaned data is then exported to the file "NYC_CityBike_data_cleaned.csv". 
Note: Due to file size limitations a copy is not located on Github.com

[NYC_CitiBike_Challenge](/NYC_CitiBike_Challenge.ipynb)

## Deliverable 2: Create Visualizations for the Trip Analysis
Using Tableau, the following Visualizations were created to display:  
* How long bikes are checked out for all riders and genders.
* How many trips are taken by the hour for each day of the week, for all riders and genders.
* A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender.


## Deliverable 3: Create a Story and Report for the Final Presentation
The full Tablue file is located on their public site, you can view the Story by using the included [link](https://public.tableau.com/app/profile/jason.smith2061/viz/Mod15Challenge/Story1) 



