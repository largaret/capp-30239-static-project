# Maggie Larson

## Description

My provisional aim for the static project is to create visualizations exploring the relationship between walkability, car ownership and voting patterns in selected U.S. regions using the EPA's National Walkability Index as a measure of walkability in combination with demographic and car ownership data included in the EPA's Smart Location Database and geospatial election results data published by the New York Times.

Transportation choices and car ownership are both political in themselves and highly constrained by politics and policy decisions; walkability is a function of the built environment, economic conditions, availability of public transit, zoning choices, etc. While the urban-rural divide has emerged as a major force in American politics, walkability and transportation choices vary significantly both between and within urban areas. I plan to explore patterns in walkability, car ownership, income levels and 2024 election results between major U.S. cities and/or across selected states, depending on the completeness and usability of data (election results data is incomplete at precinct for some states, including Illinois).

## Data Sources

### Data Source 1: EPA Smart Location Database and National Walkability Index

URL: https://www.epa.gov/smartgrowth/smart-location-mapping
Download link: https://edg.epa.gov/EPADataCommons/public/OA/EPA_SmartLocationDatabase_V3_Jan_2021_Final.csv

Size: 220,740 rows, 117 columns

The Smart Location Database (SLD) is a database compiled by the U.S. Environmental Protection Agency (EPA) summarizing demographic, employment and built environment variables at the Census block group level. This dataset includes the National Walkability Index score for each block group calculated based on the "D" variables: residential/employment density, land use diversity, design of the built environment, access to destinations, distance to transit. The SLD also includes demographic data including population count, a breakdown of workers into high-/medium-/low-income groups and number of households with 0, 1 or 2 cars.
Source: https://www.epa.gov/system/files/documents/2023-10/epa_sld_3.0_technicaldocumentationuserguide_may2021_0.pdf


### Data Source 2: NYT 2024 Election Data

URL: https://github.com/nytimes/presidential-precinct-map-2024?tab=readme-ov-file#data-dictionary
Download URL: https://int.nyt.com/newsgraphics/elections/map-data/2024/national/precincts-with-results.csv.gz

Size: 155,809 rows, 7 columns

This dataset includes precinct-level election results for the 2024 U.S. general election joined with geospatial data at precinct level. 
I plan to join this dataset with the SLD at county level using the county-level FIPS codes which are included in the GEOID variable.


## Questions

1. I'm not sure if joining the datasets at county level will be granular enough to be interesting - if not, does it seem like it would be possible to create some kind of correspondence between precincts and census block groups?