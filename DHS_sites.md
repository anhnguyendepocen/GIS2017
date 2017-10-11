# Using the DHS to complement other analyses
The [Demographic and Health Surveys](https://dhsprogram.com/) collect large household level surveys roughly every four years, depending on the country.  While the majority of the data is centered around health statistics, there is also other cross-sectoral information about things like education, land holdings, water, sanitation and hygiene, etc.  Additionally, the DHS has invested in sharing the data publicly and making it easy to incorporate into other work.  Here are the major ways they do so:


## 1. Shapefiles of [indicators](http://spatialdata.dhsprogram.com/data/#/) and [country boundaries](http://spatialdata.dhsprogram.com/boundaries/)
* Provides shapefiles for indicators for a single country, multiple countries, or all the surveys.
* You can select up to 30 separate indicators
* Data are downloaded as a shapefile or geodatabase
* Indictors are listed within the file by their [indicator code](https://api.dhsprogram.com/rest/dhs/indicators?returnFields=IndicatorId,Label,Definition&f=html)
* Additionally, they provide the country boundaries for the Administrative 1 units in a country, at the time of the survey, going back to the 1980s.
#### What should you use them for? 
* Quick maps of indicators at the Administrative 1 level
* Comparisons between countries

## 2. [Stat Compiler](https://www.statcompiler.com/en/)
* Visualize any indicator in the DHS in a table, map, or graph.
* Can select data for a particular country or countries.
* Data can be disaggregated to the Administrative 1 level, or by region (urban/rural), sex, age, education level, or asset index quntiles, where appropriate.
* Can also download the data as a .xlsx, or export figures as .pdf or .png.
* Maps can be exported as shapefiles, geodatabase, or printed.
* When exporting data, recommend using _database format_.
#### What should you use them for? 
* Visualizations of the change in indicators over time
* Visualizations of the differences in indicators between groups (among male/females, between wealth quintiles, between urban/rural, between regions, among education groups)
* Comparisons between countries

## 3. [Modelled surfaces of key indicators](http://spatialdata.dhsprogram.com/modeled-surfaces/)
* Provides a spatially modeled map surface for key demographic and health survey indicators
* Each map package contains a mean estimation surface and an uncertainty surfaces
* Can use the two surfaces to mask areas of high uncertainty (see page 41 [here](https://dhsprogram.com/pubs/pdf/SAR14/SAR14.pdf))
* Modeled surfaces have a 5 X 5 kilometer resolution
#### What should you use them for? 
  * Monitoring and evaluation specific tasks or program planning
  * Advocate for program support (identify areas of greatest need)
  * Compare program intervention areas to non-intervention areas
  * Aggregate to higher level administrative zones (Feed the Future Zones of Influence or [FEWS Net Livelihood zones](http://www.fews.net/shapefiles))
#### Things to watch out for:
  * Not good for urban areas
  * Seasonal or temporal limitations

## 4. [Raw and processed data for household surveys](https://dhsprogram.com/data/)
* Data on population, health, nutrition, HIV and for over 90 countries
* Allow for more advanced analysis, such as regression analysis (What [factors](https://github.com/flaneuse/FFP-Niger/wiki/Niger-2012-DHS-Regression-Results) are correlated with stunting in [Niger](https://dhsprogram.com/what-we-do/survey/survey-display-407.cfm)?)
* Highly standardized and structured -- slight learning curve, but once you learn how to work with the data you are good to go.
* Regularly updated and trusted
* Large user community with lots of support ([DHS Forum](https://userforum.dhsprogram.com/))
#### What should you use them for? 



## 5. [Contextual indicators at survey clusters]()
* The household surveys are collected at around 200 enumeration areas for each survey.
* To aid in bringing in other contextual indicators, the contextual data links survey cluster locations to ancillary data relating to population, climate, environment, and more.
* Detailed methodology is included in the data description file and more information about the activity can be found on [DHS's blog](https://blog.dhsprogram.com/spatial-covariates/).
#### What should you use them for? 

#### Things to watch out for:
  * If you want to create a raster surface of one of the variables, don't interpolate the cluster points.  Instead, find the data source they used so you're not essentially double interpolating.
  
 ## Other nice spatial data resources
 
