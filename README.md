## Summary
 This capstone project analyses effects of population growth on car accidents in Metropolitan and Micropolitan areas in state of TN, TX, FL, GA, and NC.
 Main goal for this analysis is to determine whether there's a correlation between 
 increase/decrease in population size and the number of total car crashes.

## Motivation
Motor Vehicle Crashes cause significant social harm and economic losses.
On average, there are 6.75 million car accidents in the U.S. every year. That’s roughly ​18,510 per day. Around 38,000 people die in automobile crashes on annual basis and an additional 3 million are injured or disabled.
Leaving in Metro Nashville area, you often hear people talk about the constant traffic accidents and how so many people are moving here every day. That made me wonder if it’s something worth looking into, if there’s any interesting patterns that can be found by combining population data with car accident reports.

## Data Sources
- [U.S Census Bureau website](https://www.census.gov/programs-surveys.html)
    * County Population Totals: 2010-2020
    * Annual Estimates of the Resident Population for Counties from April 1, 2010, to July 1, 2019, for individual states
    * Annual Estimates of the Resident Population for Counties from April 1, 2020, to July 1, 2021, for individual states
    * Core based statistical areas (CBSAs), metropolitan divisions, and combined statistical areas (CSAs)

- Crash Data Files
    * [TN Department of Safety & Homeland Security](https://www.tn.gov/safety/stats/crashdata.html)
    * [Texas Department of Transportation](https://www.txdot.gov/inside-txdot.html)
    * [Georgia Department of Transportation (GDOT)](https://gdot.numetric.net/)
    * [Florida Highway Safety and Motor Vehicles (FLHSMV)](https://www.flhsmv.gov)
    * [North Carolina Department of Transportation (NCDOT)](https://connect.ncdot.gov/resources/safety/) 
 
 
## Data Analysis and Tools
- Python
    * Analyzed “County Population totals from 2010-2020”, to identify states with the largest number of counties that fall into the top 25% of total population growth category, that are also a part of a Metropolitan Statistical Area
    * Utilized RegEx and PDFPlumber to pull crash data from state crash reports
    * Merged crashed dataframes with county population and CBSA data
    * Pandas dataframe.corr() to determine if there’s a correlation between population growth and total crashes
    
![Number of Counties by State](/visuals/top10_states.png)

- Excel
    * Data Storing

- Tableau
    * Created interactive dashboard for a more detailed overview of the data

 ## Known Issues , Challanges and Data Limitations   
* It’s important to note, that there’s multiple factors that can affect car accident crash data, however this analyses only reviews one of them.
* Census population data used in this analysis is estimate based so the final numbers might be slightly off.
* Analysis only covers 5 states.
* Data for year 2020 was excluded from correlation heatmap due to unusual behavior when included.
* Locating crash data broken down by county.
* Crash reporting differ from state to state, not to mention that some states adopted different report formatting over the years, so I had to develop an individual approach for data extraction for almost every single report.


## Tableau Dashboard



