# Title TK
This repo contains code and data for "[Title TK](URL TK)," a Center for Public Integrity story identifying the communities with existing low health insurance rates that are also likely to see a surge in newly-jobless (and thus uninsured) residents..

### Here's what's in this repo.

##### [coronavirus-jobs-losses.Rmd](coronavirus-jobs-losses.Rmd)
This R Markdown file contains code used to analyze industry employment concentration, health insurance rates and unemployment insurance claims.

##### [counties_leisure_hospitality_insurance.csv](data/exported/counties_leisure_hospitality_insurance.csv)
This CSV file contains county-level data on the number and concentration of workers in the leisure and hospitality super sector and the health insurance rate for residents. The data comes from the Bureau of Labor Statistics' [Quarterly Census of Employment and Wages](https://data.bls.gov/cew/apps/data_views/data_views.htm#tab=Tables) for the third quarter of 2019 and the Census Bureau's [Small Area Health Insurance Estimates](https://www.census.gov/data/datasets/time-series/demo/sahie/estimates-acs.html) for 2018.

##### [states_leisure_hospitality_insurance.csv](data/exported/counties_leisure_hospitality_insurance.csv)
This CSV file contains state-level data on the number and concentration of workers in the leisure and hospitality super sector and the health insurance rate for residents. The data comes from the Bureau of Labor Statistics' [Quarterly Census of Employment and Wages](https://data.bls.gov/cew/apps/data_views/data_views.htm#tab=Tables) for the third quarter of 2019 and the Census Bureau's [Small Area Health Insurance Estimates](https://www.census.gov/data/datasets/time-series/demo/sahie/estimates-acs.html) for 2018.

### Data dictionaries

##### Counties Leisure Hospitality Insurance
* area_fips: the county FIPS code
* county_name: the county name
* state_name: the state name
* pop_total: the county population from the 2018 5-year American Community Survey
* pct_non_white: the non-white and non-Hispanic share of the county's population from the 2018 5-year American Community Survey
* pct_uninsured_total: the county's total uninsured rate
* employment_leisure_hospitality: the county's number of workers employed in the leisure and hospitality super sector
* employment_leisure_hospitality_pct_total: the county's share of total workers employed in the leisure and hospitality super sector
* employment_plus_uninsured: the sum of the county's total uninsured rate and the county's share of total workers employed in the leisure and hospitality super sector
* employment_leisure_hospitality_lq: the county's [location quotient](https://www.bls.gov/cew/about-data/location-quotients-explained.htm) for the leisure and hospitality super sector

##### State Leisure Hospitality Insurance
* area_fips: the county FIPS code
* state_name: the state name
* med_exp_status: the status of Medicaid expansion in the state from the [Kaiser Family Foundation](https://www.kff.org/health-reform/state-indicator/state-activity-around-expanding-medicaid-under-the-affordable-care-act/?currentTimeframe=0&sortModel=%7B%22colId%22:%22Location%22,%22sort%22:%22asc%22%7D)
* pct_uninsured_total: the state's total uninsured rate
* pct_uninsured_138_below_poverty: the state's uninsured rate among residents aged 18 to 64 and earning 138 percent or less of the Federal poverty level
* pct_uninsured_white: the state's uninsured rate among non-Hispanic white residents
* pct_uninsured_non_white: the state's uninsured rate among the total non-white and non-Hispanic population
* pct_uninsured_black: the state's uninsured rate among non-Hispanic black residents
* pct_uninsured_hispanic: the state's uninsured rate among Hispanic residents regardless of race
* employment_leisure_hospitality: the state's number of workers employed in the leisure and hospitality super sector
* employment_leisure_hospitality_pct_total: the state's share of total workers employed in the leisure and hospitality super sector
* employment_plus_uninsured: the sum of the state's total uninsured rate and the state's share of total workers employed in the leisure and hospitality super sector
* employment_leisure_hospitality_lq: the state's [location quotient](https://www.bls.gov/cew/about-data/location-quotients-explained.htm) for the leisure and hospitality super sector