# Name

David Steffen

# Topic

I am planning to build an interactive visualization of health insurance coverage rates that will allow users to explore health insurance coverage at the national, state, and (possibly) county-level.

The first choice a user can make is which topic they are interested in exploring health insurance coverage rates by, between: <br>
&ensp; Race/ethnicity <br>
&ensp; Insurance type <br>
&ensp; Income <br>

Once a choice has been made, the user can use a Selection dropdown based on the topic to select a "level", which would allow them to explore geographic differences in health insurance rates for that population or insurance type <br>
&ensp; Race/ethnicity: White, Black, Hispanic, Asian <br>
&ensp; Insurance type: private, public, no insurance, Medicaid <br>
&ensp; Income: based on % of Federal Poverty Level (FPL) <br>

I think that for some of the levels, or possibly all levels depending on data availability, there also could be a second dropdown for age group as well (e.g., <19 vs. 19-34 vs. 35-64). Based on my review of the available data, what age groups have data available will be different for different selections.

The national level map will then populate and color based on the health insurance coverage rate for the level the user has selected (see first mockup below).

Users could then select a state to filter down to its data, which would also display data for the selected level (maybe at the county level, see second mockup below).

I am also considering adding additional visualizations on the state-level views comparing to the national level, though I'm less sure of what this would look like (I included one possibility in the mockup).

I think this is most similar to Option A.

# Data I plan to use

The two main data sources will be tables from the American Community Survey (ACS) 1-year and 5-year estimates, and from the Kaiser Family Foundation (KFF).

**Race/Ethnicity**

ACS B27001 <br>
&ensp; Types: Only "with health insurance" vs. "no health insurance" <br>
&ensp; Age groups: at 10 year level <br>
&ensp; Breakdowns: Available for each race/ethnicity <br>
&ensp; Estimates: 1-year and 5-year for overall, 1-year only for race/ethnicity groups <br>
&ensp;&ensp; (C27001 has the same with 5-year estimates) <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27001 <br>

KFF
&ensp; Uninsured Rates for People Ages 0-64 by Race/Ethnicity <br>
&ensp;   https://www.kff.org/uninsured/state-indicator/people-0-64-uninsured-rate-by-raceethnicity/ <br>
&ensp; Employer-Sponsored Coverage Rates for People Ages 0-64 by Race/Ethnicity <br>
&ensp;   https://www.kff.org/other/state-indicator/people-0-64-employer-coverage-rate-by-raceethnicity/ <br>
&ensp; Medicaid Coverage Rates for People Ages 0-64 by Race/Ethnicity <br>
&ensp;   https://www.kff.org/medicaid/state-indicator/people-0-64-medicaid-rate-by-raceethnicity/ <br>
&ensp; Health Insurance Coverage of Population Ages 0-64 (overall % in each by state) <br>

**Insurance Type**

ACS B27002-B27009 <br>
&ensp; Types: each of "with type" vs. "without type" for Medicaid, public, etc. <br>
&ensp; Age groups: at 10 year level <br>
&ensp; Estimates: 1-year <br>
&ensp;&ensp; (C27002-C27009 has the same with 5-year estimates, less categories) <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27002 <br>

ACS B27010
&ensp; Types: each type of insurance, including combinations, all in one table <br>
&ensp; Age groups: <19, 19-34, 35-64 <br>
&ensp; Estimates: 1-year and 5-year <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27010 <br>

ACS C27010 <br>
&ensp; Types: mutually exclusive private/public/both/none <br>
&ensp; Age groups: <19, 19-34, 35-64 <br>
&ensp; Estimates: 1-year <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.C27010 <br>

**Income**
ACS B27018-B27019 <br>
&ensp; Types: private and public <br>
&ensp; Age groups: <19, 19-64 <br>
&ensp; Breakdowns: <0.5, 0.5-.99, 1-1.38, 1.38-1.49, 1.5-1.99, etc. to 4+ of FPL <br>
&ensp; Estimates: 1-year <br>
&ensp;&ensp; (C27017-27018 have broader categories but 5-year estimates) <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27018 <br>

ACS S2703-S2704 <br>
&ensp; Number and percent in private and public <br>
&ensp; Breakdowns <br>
&ensp;&ensp; below/above 138% of FPL <br>
&ensp;&ensp; Age groups at 10 year level <br>
&ensp; Estimates: 1-year and 5-year <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.S2703 <br>

# Examples of kinds of interactive visualization I am considering

A few of the example visualizations inspired my idea to allow users to select aspects of particular interest (for these, year, for me, topic/subpopulation). The NYT visualization also allows users to select a geographic area of interest, which I will also do (for them, hometown, for me, state). <br>
&ensp;  https://www.nytimes.com/interactive/2018/08/30/climate/how-much-hotter-is-your-hometown.html <br>
&ensp;  https://www.nature.org/en-us/get-involved/how-to-help/carbon-footprint-calculator/carbon-by-birth-year/ <br>

A few of the example visualizations inspired my idea of using a map, highlighting particular areas, then having more information populate as you zoom in on a particular area. <br>
&ensp; https://especiales.eldiario.es/spain-lives-in-flats/ <br>
&ensp; https://wfca.com/fire-map <br>

Another such example I found that allows selection at the county level and then populates graphs and information: <br>
&ensp; https://www.nytimes.com/interactive/2016/04/11/upshot/where-the-poor-live-longer-how-your-area-compares.html

# Questions

1. Do you think that this would benefit from county-level data, or do you think state-level visualizations would suffice? One caveat is that some variables/tables (those labeled "1-year estimates" above) are only available for counties with >65,000 people, so this would limit what data I could display.

2. More generally, do you think this is of an appropriate scope? Are there any changes you would suggest to the scope I proposed in either direction?

3. On the state-level view, if I do not include county-level data, do you have any suggestions for what else I could display on the state outlines instead?

4. On the state-level view, how would you recommend comparing to the national level?

# Image files of mock-ups

[National-Level](scratch/mockup_1.jpg)

[State-Level](scratch/mockup_2.jpg)
