# Name

David Steffen

# Topic

I am planning to build an interactive visualization of health insurance coverage rates that will allow users to explore health insurance coverage at the national, state, and (possibly) county-level.

The first choice a user can make is which topic they are interested in exploring health insurance coverage rates by, between: <br>
&ensp; Race/ethnicity <br>
&ensp; Insurance type <br>
&ensp; Income <br>

Once a choice has been made, the user can use a Selection dropdown based on the topic to select a "level" <br>
&ensp; Race/ethnicity: White, Black, Hispanic, Asian <br>
&ensp; Insurance type: private, public, no insurance, Medicaid <br>
&ensp; Income: based on % of Federal Poverty Level (FPL) <br>

I think that for some levels, there also could be a second dropdown for age group as well (e.g., <19 vs. 19-34 vs. 35-64).

The national level map will then populate and color based on the health insurance coverage rate for the level the user has selected.

Users could then select a state to filter down to its data, which would also display data for the selected level (maybe at the county level).

I am also considering adding additional visualizations on the state-level views comparing to the national level, though I'm less sure of what this would look like.


# Data I plan to use

**Race/Ethnicity**

B27001 <br>
&ensp; Types: Only "with health insurance" vs. "no health insurance" <br>
&ensp; Age groups: at 10 year level <br>
&ensp; Breakdowns: Available for each race/ethnicity <br>
&ensp; Estimates: 1-year and 5-year for overall, 1-year only for race/ethnicity groups <br>
&ensp;&ensp; (C27001 has the same with 5-year estimates) <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27001 <br>

KFF
&ensp; Uninsured Rates for People Ages 0-64 by Race/Ethnicity <br>
&ensp; Employer-Sponsored Coverage Rates for People Ages 0-64 by Race/Ethnicity <br>
&ensp; Medicaid Coverage Rates for People Ages 0-64 by Race/Ethnicity <br>
&ensp; Health Insurance Coverage of Population Ages 0-64 (overall % in each by state) <br>

**Insurance Type**

B27002-B27009 <br>
&ensp; Types: each of "with type" vs. "without type" for Medicaid, public, etc. <br>
&ensp; Age groups: at 10 year level <br>
&ensp; Estimates: 1-year <br>
&ensp;&ensp; (C27002-C27009 has the same with 5-year estimates, less categories) <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27002 <br>

B27010
&ensp; Types: each type of insurance, including combinations, all in one table <br>
&ensp; Age groups: <19, 19-34, 35-64 <br>
&ensp; Estimates: 1-year and 5-year <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27010 <br>

C27010 <br>
&ensp; Types: mutually exclusive private/public/both/none <br>
&ensp; Age groups: <19, 19-34, 35-64 <br>
&ensp; Estimates: 1-year <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.C27010 <br>

**Income**
B27018-B27019 <br>
&ensp; Types: private and public <br>
&ensp; Age groups: <19, 19-64 <br>
&ensp; Breakdowns: <0.5, 0.5-.99, 1-1.38, 1.38-1.49, 1.5-1.99, etc. to 4+ of FPL <br>
&ensp; Estimates: 1-year <br>
&ensp;&ensp; (C27017-27018 have broader categories but 5-year estimates) <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.B27018 <br>

S2703-S2704 <br>
&ensp; Number and percent in private and public <br>
&ensp; Breakdowns <br>
&ensp;&ensp; below/above 138% of FPL <br>
&ensp;&ensp; Age groups at 10 year level <br>
&ensp; Estimates: 1-year and 5-year <br>
&ensp; https://data.census.gov/table/ACSDT1Y2023.S2703 <br>

# Examples of the kinds of interactive visualization I am considering


# Questions

1. Do you think that this would 

# Image file of mock-up

[National-Level](scratch/mockup 1.heic)

[State-Level](scratch/mockup 1.heic)
