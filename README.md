# Baltimore 911 Data Report  

As part of Data mining class, we were asked to make an interactive Dashboard to analyze the data of 911 calls report of Baltimore City. It contains details like Crime Types, location, District, Weapons, total crime numbers etc. 

## Explorative Data Analysis

### Data measurement:

Found the mean, mode, median and standard deviation of the numerical data types including: 'Post', 'Longitude', 'Latitude', 'Total Incidents'.

### Finding the missingness in the data:

```
missingness = df.isnull().sum() / total_rows * 100
```

### Data Cleaning:

```
data_cleaned = data.dropna(subset=['CrimeDate', 'CrimeCode', 'Description', 'Total Incidents'])
```

There were numerous `Nan` data in the columns, with the help of Data Wrangling I cleaned the file and replaced them with `Unknown` for the categorical data types. 

As a result, with the help of Python and Tableau I created an interactive Dashboard that can show the Data based on the filters including:
- Crime Date (year)
- Crime Date (Day of the month)
- Crime Date (Day of the week)
- Crime type
- Crime Location (Location and District)

