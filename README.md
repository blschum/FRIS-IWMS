# FRIS-IWMS

<<<<<<< HEAD
Climate change is projected to transform US agriculture, particularly in places reliant on limited irrigation water resources. As water demand and scarcity increase simultaneously over the coming decades, water managers and growers will need to optimize water use on their irrigated lands. Understanding how growers maintain high yields in arid, water stressed places, while conserving water, is of key importance for the future of US agriculture in the West. We explore water use management and trends in irrigated agriculture in the West using operator-level USDA-NASS Farm and Ranch Irrigation Survey/Irrigation and Water Management Survey data aggregated for the first time to the county-scale. In this exploration, we build the first county-level, openly accessible dataset linking farm(er) characteristics to irrigation behaviors in the West. We find notable spatial and temporal variability in Western irrigation practices, with neighboring counties exhibiting large differences in efficiency, water use, and crop yields, as well as in the sources of information, scheduling methods, and technological improvements employed. To produce effective management initiatives in the West, we call for the express and open dissemination of USDA irrigation data at sub-state scales. These data will contribute to our understanding of irrigated production and could support a pathway that will prepare growers for a more resilient agricultural future. 
=======
Climate change is projected to transform US agriculture, particularly in places reliant on limited irrigation water resources. As water demand and scarcity increase simultaneously over the coming decades, water managers and growers will need to optimize water use on their irrigated lands. Understanding how growers maintain high yields in arid, water stressed places, while conserving water, is of key importance for the future of US agriculture in the West. We explore water use management and trends in irrigated agriculture in the West using operator-level USDA-NASS Farm and Ranch Irrigation Survey/Irrigation and Water Management Survey data aggregated for the first time to the county-scale. In this exploration, we build the first county-level, openly accessible dataset linking farm(er) characteristics to irrigation behaviors in the West. We find notable spatial and temporal variability in Western irrigation practices, with neighboring counties exhibiting large differences in efficiency, water use, and crop yields, as well as in the sources of information, scheduling methods, and technological improvements employed. To produce effective management initiatives in the West, we call for the express and open dissemination of USDA irrigation data at sub-state scales. These data will contribute to our understanding of irrigated production and could support a pathway that will prepare growers for a more resilient agricultural future. 

## Getting started

If you've stumbled up on this repo and are interested in the FRIS/IWMS data we produced, or the code we built, please see the descriptions below of each dataset and each .Rmd/.html file:

### Data files in FRIS-IWMS/data

‘alfalfa_SDcat.RDS’: creates bins for counties that are above +1SD, below -1SD and within +1SD/-1SD of irrigation productivity, estimated average water use, and estimated average yield in 2018. Includes columns used to find these bins. Also includes the column ‘unique’ which shows the number of unique STPOIDs summarised across and the maximum yield and water use in US measurements. Irrigation productivity is simply a ratio of yield/water used.

‘assist_prop_allyrs.RDS’: the proportion of responses in each assistance category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs across the 2013 IWMS and 2018 FRIS years (combined).

‘assist_prop_indyrs.RDS’: the proportion of responses in each assistance category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs for individual years.

‘bar-assist-chisq.csv’: the proportion of responses across assistance categories (yes/no) across years.

‘barrier_prop_allyrs.RDS’: the proportion of responses in each barrier category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs across the 2013 IWMS and 2018 FRIS years (combined).

‘barrier_prop_indyrs.RDS’: the proportion of responses in each barrier category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs for individual years.

‘bw_panel_stats.RDS’: the median and standard deviation of yield, water use, and irrigation productivity across the panel dataset for each crop.

‘bw_st_stats.RDS’: the lower, middle, and upper bound of the box plot, plus the median and standard deviation of yield, water use, and irrigation productivity for each crop-year-state combination. Will use to discuss differences across crops-years-states.

‘bw_yr_stats.RDS’: the lower, middle, and upper bound of the box plot, plus the median and standard deviation of yield, water use, and irrigation productivity for each crop-year combination. Will use to discuss differences across crop-years.

‘county.RDS’: R spatial file of US counties in coterminous US.

‘cty_names.RDS’: county names file for matching and visualization datasets.

‘full_merged_irrigation.RDS’: interpolated irrigation data for the coterminous US.

‘info-assist-chisq.csv’: the proportion of responses across assistance categories (yes/no) across years.

‘info_prop_allyrs.RDS’: the proportion of responses in each information source category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs across the 2013 IWMS and 2018 FRIS years (combined).

‘info_prop_indyrs.RDS’: the proportion of responses in each information source category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs for individual years.

‘sched_prop_allyrs.RDS’: the proportion of responses in each scheduling method category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs across the 2013 IWMS and 2018 FRIS years (combined).

‘sched_prop_indyrs.RDS’: the proportion of responses in each scheduling method category (weighted by ‘statwij’) summarised at n >= 6 unique STPOIDs for individual years.

‘states.RDS’: R spatial file of US states in coterminous US.

‘sumstat_allyrs.RDS’: estimated average yield, estimated average water used, estimated average irrigation productivity summarised at county-crop n >= 6 unique STPOIDs across all years. Includes the column ‘unique’ which shows the number of unique STPOIDs summarised across and the maximum yield and water use in US measurements. Irrigation productivity is simply a ratio of yield/water used.

‘sumstat_indyrs.RDS’: estimated average yield, estimated average water used, estimated average irrigation productivity summarised at county-crop n >= 6 unique STPOIDs across individual years (a fake example: Berks County, PA might have 14 irrigators in 2013, but only 9 in 2018–in 2018 the data will be suppressed and Berks will show as ‘NA’, in 2013, we will have the estimated average across those 14 irrigators). Includes the column ‘unique’ which shows the number of unique STPOIDs summarised across and the maximum yield and water use in US measurements. Irrigation productivity is simply a ratio of yield/water used.

‘western_ctys.RDS’: R spatial file for 11 western-most states' counties in coterminous US.

### .RDS/.html files in FRIS-IWMS

>>>>>>> 863f97df368d552e4653ea010b32faece371b243
