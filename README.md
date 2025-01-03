# LA-Crime-Trends-Pre-Post-COVID

A data-focused project investigating crime trends in Los Angeles from 2010 to the present, with special emphasis on analyzing how the COVID-19 pandemic may have influenced both overall crime rates and the proportions of crime types (violent, property, and sex crimes).

---

## Table of Contents
[Overview](#overview)  
[Analysis Summary](#analysis-summary)  
[Further Research](#further-research)  
[References](#references)

---

## Overview
This repository contains a self-contained R Markdown document and its corresponding HTML output. The analysis demonstrates:
- Data cleaning and categorization of crime incidents (violent, property, and sex crimes).
- Statistical tests (difference of proportions, Welch Two-Sample t-test) to investigate potential shifts in crime patterns before and after the onset of the COVID-19 pandemic.
- Exploratory graphs illustrating trends over time.

---

## Analysis Summary

1. **Time Series Examination**:  
   - Plots illustrating monthly/yearly crime counts from 2010 to the present.  
   - Demonstrates a dip in total crimes around 2020.

2. **Statistical Testing**:  
   - **Difference of Proportions Test**: Suggests there is a **significant** difference in the proportion of violent crimes pre-COVID vs. post-COVID.  
   - **Welch Two-Sample T-Test**: Shows **no** statistically significant difference in the *average monthly total* of reported crimes before vs. after the onset of COVID-19.

3. **Interpretation**:  
   - While overall crime rates did not significantly change, there is a noteworthy shift in *type* (violent vs. non-violent) across the two periods.

---

## Further Research
1. **Longer Post-COVID Data Window**: Extending the timeline beyond early 2024 could offer additional clarity.  
2. **Socioeconomic Indicators**: Incorporate data on unemployment rates, housing statistics, or public health restrictions to further interpret crime trends.  
3. **Geospatial Analysis**: Analyzing regional differences within Los Angeles could reveal specific hotspots or patterns.  

---

## References
1. **Crime Data from 2010 to 2019**  
   [Crime Data from 2010 to 2019](https://catalog.data.gov/dataset/crime-data-from-2010-to-2019)

2. **Crime Data from 2020 to Present**  
   [Crime Data from 2020 to Present](https://catalog.data.gov/dataset/crime-data-from-2020-to-present)

3. **National Library of Medicine**  
   [NCBI Article on COVID-19-related impacts in Los Angeles](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7996058/)
---

**Disclaimer**:  
These findings are based on *reported* crime incidents only. Interpretations should be made cautiously, as unreported crimes and variations in reporting practices could influence results.  
