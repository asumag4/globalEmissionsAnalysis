<img src="https://media.hswstatic.com/eyJidWNrZXQiOiJjb250ZW50Lmhzd3N0YXRpYy5jb20iLCJrZXkiOiJnaWZcL2Fpci1wb2xsdXRpb24tMS5wbmciLCJlZGl0cyI6eyJyZXNpemUiOnsid2lkdGgiOjgyOH0sInRvRm9ybWF0IjoiYXZpZiJ9fQ==" alt="road-emissions" />
# Global Road Emissions Analysis 

Comprehensive study consisting of 6 datasets from 5 sources, studying the relationship of road emissions on global economy, life expectancy, cancers and temperature anomalies

## About the Data 

**Sources:**

Emissions Data from <a href="https://climatetrace.org/data#:~:text=Climate%20TRACE%20emissions%20data%20are,information%20on%20our%20beta%20API">climatetrace.org</a>
Life Expectacny data from <a href="https://data.who.int/indicators/i/48D9B0C/C64284D">World Health Organization</a>
GDP Data from <a href="https://data.worldbank.org/indicator/NY.GDP.PCAP.CD">worldbank.org</a>
Cancer Rates data from <a href="https://ghdx.healthdata.org/">Global Health Data Exchange</a>
Monthly Temperature Anomalies from <a href="https://ourworldindata.org/grapher/monthly-temperature-anomalies">Our World in Data</a>

## Analysis and Conclusions 

Data was cleaned, removed of null values on any row and pivotted for a homogenous format (ex: one column for 'year', one column for 'country', renaming of country code column header)

Used SQL and python SQL connector to query between the datatables. 

We determined the following relationships between the variables-of-study: 
1. A general positive relationship between GDP and Road/ Transportation Emissions
2. Most countries display a significant correlation between transportation emissions and respiratory cancers
3. Some countries adopt cleaner technologies, producing higher GDP but with lower emissions and temperature anomalies than other less-developed countries. Thus indicating that innovation can be gauged by these three factors.
4. No trend between road emissions and life expectancies.
5. Certain countries display a strong relationship between Life Expectancy and GDP, and vice versa. When investigated with proportion of GDP spent on healthcare vs. life expectancy, there was a weak significant correlation discovered.

## Future Steps 
1. A more comprehensive and targetted study should be conducted
2. Improve data importation from python to SQL
