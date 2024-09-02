# Covid_data_analysis
![image](https://github.com/user-attachments/assets/64be24a5-b1a5-43d7-9eb7-593ad4b4f03b)

### ECDC_COVID_19:DATASET DESCRIPTION

* dateRep: The date of the reported data

* day: The day of the report (integer, e.g., 1-31).

* month: The month of the report (integer, e.g., 1-12).

* year: The year of the report (integer, e.g., 2020).

* cases: The number of new confirmed cases reported on this date.

* deaths: The number of new deaths reported on this date.

* countriesAndTerritories: The name of the country or territory to which the data belongs.

* geoId: A short geographical identifier (code) for the country or territory.

* countryterritoryCode
  
## Information of the Dataset

* Columns = 10
* Rows = 9513
* Data types
    - float -1
    - integer - 5
    - object - 4
* Occur Null values
    - geoId - 25
    - countryterritoryCode - 189
    - popData2018 - 143
* No duplicate values

## Questions :
* filtering and sort
1) filter the dataset to include only rows where the countriesandterritories column is either united_states_of_america or india?
2) filter the dataframe to include only the rows where the month column is either january or february
3) select the rows where geoid is not in a list of excluded codes (excluded_codes=['US','IN','BR'])?
4) Filter rows where the countriesAndTerritories column contains 'Germany','France','Italy'.
5) Filter out rows where the countriesAndTerritories column not contains 'Germany','France','Italy'.
6) extract geoid HR,CU,CW,CY -- reindex,year wise indexing
7) extract countries and territory code = GVR, KNA, NLD, PRT --set index in day_name base
8) filter the rows where cases>1000 and deaths>500
9) set_index is month_name and sort in descending
* pivot table()
1) create a pivot table that summarizes the total number of deaths for each country, broken down by month
2) create a pivot table that shows the average number of deaths per country for each month
3)  create a pivot table that summarizes the total number of deaths for each country, broken down by year
4)  create a pivot table that displays the average population data for each country across different years
5)  create a pivot table that shows the maximum number of cases recorded for each country in each year
6)  create a pivot table that displays the maximum number of cases recorded for each country during each month
7)  create a pivot table that shows the total number of deaths for each geographical region, broken down by each day of the week
* melt()
1)  reshape a DataFrame to unpivot the 'cases' and 'deaths' columns into a single column, while keeping the countries and territories and reported date information intact
* groupby()
1)  find the maximum number of deaths recorded for each country or territory in the DataFrame
2)  calculate the average number of cases for each country or territory in the DataFrame
3)  calculate the total number of deaths for each country or territory for each year in the DataFrame
4)  find the average population data for the year 2018 for each country or territory in the DataFrame
5)  determine the maximum number of cases and the minimum number of deaths for each country or territory in each year in the DataFrame
6)  find the minimum, maximum, and average population data for the year 2018 for each country or territory in each year in the DataFrame
7)  find the maximum population data for 2018 and the total number of cases for each combination of date, day, month, and year in the DataFrame
* apply()
1)  create a new column in the DataFrame that adds 5 to the value in the 'popData2018' column for each row
2)  create a new column in the DataFrame that adds 5 to each value in the 'deaths' column
* idxmax()
1)   identify the row with the maximum number of deaths in your dataset
2)   Which country or territory has the lowest minimum death count in the dataset?
3)   Which row in the dataset corresponds to the lowest number of deaths, and what are the details of that row
4)   Which month has the highest maximum number of cases recorded across all months in the dataset
* cut()
1)   categorize the number of deaths in your dataset into different levels such as 'Low,' 'Medium,' 'High,' and 'Very High'

   
