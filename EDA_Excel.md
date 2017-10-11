### Exploratory Data Analysis using Excel
* Define your analytical question: What is the primary question you would like to answer with the data?
  * What are the trends in HIV positivity rates for the last four quarters?
  * Are there any particular clinics or geographic regions that stand out?

##### Checking the Data
###### Variables
* Variable names
  * Consistent?
  * Understandable?
* Variable types
  * Numeric or text (strings)
  * `type` command will reveal data types  

###### Missing values -
* Nature of missing values [not a trivial issue](http://www.lexjansen.com/nesug/nesug01/ps/ps8009.pdf)
  * How are the values missing?
  * Blank, NA, NaN, 9999, -999, refused to answer etc.
* Excel tools
  * `countif` - count number of cells meeting a condition
  * `countblank` -  count number of empty cells

###### Outliers
* value that is abnormally different from other values
    * geographic
      * latitude/Longitude range
      * admin values correct
    * Numeric
      * percentages greater than 100%
      * abnormal values
    * Text
      * Inconsistent spelling
      * Dates formatted inconsistently

###### Unique Identifiers / Duplicate values
* unique ID - allow one to uniquely identify an observation
* duplicates -

##### Pivot Tables for Data Cleaning
###### What is a pivot table?
* tool to reorganize and summarize spreadsheet data
* does not change the raw/original data
* allows for rapid filtering, sorting, summarizing

###### Creating a pivot table
1. navigate to ribbon, select `insert`
2. click `PivotTable` and select range of values
3. select `New Worksheet` for placement location
4. a new worksheet will open with a blank table
5. explore the ribbon and PivotTable Fields

----
#### Data Cleaning Tasks:
1. Check latitude/longitude values
2. Filter the data by `SNU1 == gp Gauteng Province` and count the number of facilities
3. Find all facilities where `rate > 100`
4. Look at 

