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
1) filter the dataset to include only rows where the countriesandterritories column is either united_states_of_america or india?
2) filter the dataframe to include only the rows where the month column is either january or february
3) select the rows where geoid is not in a list of excluded codes (excluded_codes=['US','IN','BR'])?
4) Filter rows where the countriesAndTerritories column contains 'Germany','France','Italy'.
5) Filter out rows where the countriesAndTerritories column not contains 'Germany','France','Italy'.
6) extract geoid HR,CU,CW,CY -- reindex,year wise indexing
7) extract countries and territory code = GVR, KNA, NLD, PRT --set index in day_name base
8) filter the rows where cases>1000 and deaths>500
9) set_index is month_name and sort in descending
   
