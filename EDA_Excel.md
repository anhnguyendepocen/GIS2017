# Lessons from Exploratory Data Analysis:
1. **Why?** Exploratory data analysis is useful to:
    * assess the quality of your data
    * learn about your data
    * analyze your data
2. **What?** Check each type of data _before_ you analyze it
    * geographic 
    * categorical
    * numeric
3. **How?** Plotting, filtering, and sorting are your three tools to explore your data

 
 
## Exploratory Data Analysis using Excel
* Define your analytical question: What is the primary question you would like to answer with the data?
  * What are the trends in HIV positivity rates for the last four quarters?
  * Are there any particular clinics or geographic regions that stand out?

## Checking the Data
### Variables
* Variable names
  * consistent?
  * understandable?
* Variable types
  * numeric or text (strings)
  * `type` command will reveal [data types in Excel](https://support.office.com/en-us/article/TYPE-function-45b4e688-4bc3-48b3-a105-ffa892995899)

### Missing values
* nature of missing values [not a trivial issue](http://www.lexjansen.com/nesug/nesug01/ps/ps8009.pdf)
  * how are the values missing?
  * blank, NA, NaN, 9999, -999, refused to answer etc.
* Excel tools
  * `countif` - count number of cells meeting a condition
  * `countblank` - count number of empty cells

### Outliers
* value that is abnormally different from other values
    * geographic
      * latitude/longitude range
      * admin values correct
    * numeric
      * percentages greater than 100%
      * abnormal values
    * text
      * Inconsistent spelling
      * Dates formatted inconsistently

### Unique Identifiers / Duplicate values
* unique ID - allow one to uniquely identify an observation
* duplicates - if not identified, derived values will be potentially flawed (double-counting)
* `Table` - convert data to a table and use `Remove Duplicates` command to scan data for duplicates   

## Pivot Tables for Data Cleaning
### What is a pivot table?
* tool to reorganize and summarize spreadsheet data
* does not change the raw/original data
* allows for rapid filtering, sorting, summarizing

### Creating a pivot table
1. navigate to ribbon, select `insert`
2. click `PivotTable` and select range of values
3. select `New Worksheet` for placement location
4. a new worksheet will open with a blank table
5. explore the ribbon and PivotTable Fields

### Understanding the PivotTableFieldList
* `Fields` - variables in your dataset
* `Filter` - filter variables based on values
* `Column` - variables that will appear in the column  
* `Row` - variables that will appear in the rows  
* `Values` - summarized numeric values

## Data Cleaning Tasks:
1. check latitude/longitude values
2. filter the data by `SNU1 == gp Gauteng Province` and count the number of facilities
3. find all facilities where `rate > 100`
4. create a summary table showing the rate variable for each facility, by quarter

## Resources  
[PEPFAR Examples](https://achafetz.github.io/pals_dataviz/)  
[Bar Graphs](https://geocenter.github.io/resources/2016/10/26/bargraph.html)  
[Heatmap](https://geocenter.github.io/resources/2016/10/12/heatmap.html)  
[Stephanie Evergreeen Blog](http://stephanieevergreen.com/blog/)  
[GitHub](https://github.com)  

 
