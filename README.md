# DA_project

### Problem statement:
---
Which percentages of special population groups correlate with the Overall Scaled Score at the district level? 

### Data & Process (cleaning and transforming)
---
- StudPgmStateDistrict 2018-19: 

To do the calculation - I dropped columns, removed the -999 values, and replaced them with zeros. Calculated percentages and added the additional columns to the dataframe. 

-  DISTRATE 2018-2019: 

For this dataset, I loaded only columns needed for the calculating correlation and merging (DDALLS, D_RATING, & REGION)
The missing values were only in the DISTRATE 2018-2019 dataset, and those columns were not needed therefore not loaded for the analysis.

### Limitations seen in the data
---
The datasets contained the necessary information for the task. However, including additional data might have been helpful to establish more of a trend for a time series analysis. In analyzing the different student populations for the regions, future data collection should include data for refugees and students employed to help support their families (parents).

StudPgmStateDistrict 2018-19.xls dataset includes a brief description of the population groups. The information on the following URL was helpful for the other datasets analysis https://rptsvr1.tea.texas.gov/adhocrpt/Standard_Reports/About/About_StudentProgram.html.


### Observations
---
Many groups had several entries with -999 that symbolized protected data.
Foster care: 473, Military connected: 460, Homeless: 310, Dyslexic: 217
For the histograms 
- %AT RISK is distributed slightly positively and 
- %ECONOMICALLY DISADVANTAGED is also normally distributed but slightly negative.
- As expected, based on masked values and histograms %MILITARY CONNECTED and %FOSTER CARE are highly skewed (positively).
- Scatter plots - the language populations (%BILINGUAL, %EMERGENT BILINGUAL/ENGLISH LEARNER, %ESL) are similarly shaped in relationship to DDALLS.
- From the heatmap, there is a negative correlation comparing DDALLS with the %GIFTED & TALENTED, %BILINGUAL, %EMERGENT BILINGUAL/ENGLISH LEARNER, %CTE, %ESL population groups. 
- The population group for %HOMELESS is slightly negatively correlated. 

The number of masked values in the data might be the cause of the skewness and negative correlation, and additional data might help to determine if that is the case.

