# Walkability in five major US cities

Maggie Larson

## What is your current goal? Has it changed since the proposal?
My current goal is to compare walkability across five different metropolitan areas in the US, looking specifically at the core-based statistical areas, or CBSAs, containing New York City, Los Angeles, Chicago, Dallas and Houston. Some of the factors I plan to include in the final visualizations are the geographic layout of the metro areas, wealth, car ownership and 2020 election outcomes. (This is a change from the proposal - I was originally looking at 2024 election data, but have instead chosen 2020 since the national walkability index (NWI) numbers I'm using were calculated in 2021.) The overall aim is to highlight differences in walkability and transportation patterns in these cities.

## Are there data challenges you are facing? Are you currently depending on mock data?
All of the data used in the current visualizations is real data. The main challenge currently is finding the right level of granularity for effective visualizations - for each city there are thousands of block-level observations of varying population size and geographic size, which are both hard to visualize and difficult to compare directly. This also poses technical challenges for loading and analyzing data and generating visualizations. I am exploring different grouping approaches to reduce the number of rows.

## Describe each of the provided images with 2-3 sentences to give the context and how it relates to your goal.

#### How many people live in walkable areas?
![NWI by population](imgs/nwi_by_population_by_cbsa.png)
Type: bar chart
This shows the population distributed over the EPA National Walkability Index (NPI) scores in each of the metro areas. This chart gives a broad overview of how many people live in more walkable areas in each city, while also visually preserving the difference in population between CBSAs.

![NWI density chart, NY](imgs/nwi_pop_density_ny.png)
![NWI density chart, LA](imgs/nwi_pop_density_la.png)
![NWI density chart, CHI](imgs/nwi_pop_density_chi.png)
![NWI density chart, HOU](imgs/nwi_pop_density_hou.png)
![NWI density chart, DAL](imgs/nwi_pop_density_dal.png)
Type: line graph (density function)
These density graphs should be displayed with or possibly overlaid on the previous bar chart; for each city, they show a density function of population over the NWI score range. This more clearly shows differences in distribution between the CBSAs - the shape of the distributions for Houston and Dallas are notably different from those for New York and LA, for example.

![NWI stacked proportions](imgs/nwi_stacked_by_cbsa.png)
Type: stacked bar chart
This shows a direct comparison of the proportion of each city's population living in walkable areas.

#### Walkable areas vote blue (or, blue areas are more walkable)

![NWI vs 2020 vote by county](imgs/nwi_v_dem.png)
Type: scatter plot
This shows NWI score vs percentage 2020 Democratic lead for each county in the five CBSAs, color-coded by metro area. This shows a clear linear relationship between the two: more walkable counties are more Democratic. This isn't intended to suggest a causal relationship between the two, but I think the strength of the relationship is an interesting part of the story.

![NWI map, DAL](imgs/nwi_map_dal.png)
![2020 vote map, DAL](imgs/2020_map_dal.png)
Type: map (geo_shape)
These two maps side-by-side present a comparison between walkability index (at block group level) and 2020 voting (at precinct level) in the Dallas metro area. The relationship between the two is particularly clear here, since you can see pockets of brighter (more walkable) areas on the walkability map corresponding to pockets of blue on the voting map.

#### I'm walking here: car ownership is lower in New York

![auto ownership by CBSA](imgs/autoown_by_cbsa.png)
Type: bar chart
This shows the proportion of households in each metro area which own zero, one or two or more cars; the New York area is a notable exception. Even though the distribution of people living in walkable areas in New York and LA are similar, car ownership patterns are very different. (I hope to display this somewhat differently in the final version to highlight New York as an outlier.)

![](imgs/autoown_piechart.png)
![](imgs/nwi_map_nyc.png)
Type: map, pie chart (!)
These charts focus specifically on the five boroughs of New York City, making a connection between the high walkability scores of the boroughs and low car ownership.

![](imgs/nwi_v_autoown_heatmap.png)
Type: heatmap
This shows a heatmap of car ownership by NWI score for all CBSAs.

#### Wealth and walkability in Chicago

![](imgs/nwi_map_chi_cook.png)
![](imgs/2020_map_chi_cook.png)
![](imgs/wealth_map_chi_cook.png)
Type: map
These three maps of Cook County show walkability, 2020 voting patterns and the percentage of households categorized as low-wage by block group. Together, they show a political and economic divide between the more walkable, wealthier north side of the city and the less walkable south side.

#### Transit patterns

![](imgs/d4ar_chi_cook.png)
![source: https://gisgeography.com/chicago-map-illinois/](Chicago-Road-Map-1000x1294.jpg)
Type: map
This map shows the number of jobs within a 45-minute commute by car in Cook County. This illustrates how well different parts of the city are connected by road to the economic center of Chicago; I plan to compare this to a similar map showing public transit commutes.


## What form do you envision your final narrative taking? (e.g. An article incorporating the images? A poster? An infographic?)
I envision the final output of this project as an infographic showing both broad comparisons between the five cities and explorations of features of the individual cities.