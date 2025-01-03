# LA-Crime-Trends-Pre-Post-COVID

# LA-Crime-Trends-Pre-Post-COVID

A data-focused project investigating crime trends in Los Angeles from 2010 to the present, with special emphasis on analyzing how the COVID-19 pandemic may have influenced both overall crime rates and the proportions of crime types (violent, property, and sex crimes).

---

## Table of Contents

1. [Overview](#overview)  
2. [Files in This Repository](#files-in-this-repository)  
3. [Data Requirements](#data-requirements)  
4. [Usage](#usage)  
5. [Analysis Summary](#analysis-summary)  
6. [Further Research](#further-research)  
7. [References](#references)

---

## Overview
This repository contains a self-contained R Markdown document and its corresponding HTML output. The analysis demonstrates:
- Data cleaning and categorization of crime incidents (violent, property, and sex crimes).
- Statistical tests (difference of proportions, Welch Two-Sample t-test) to investigate potential shifts in crime patterns before and after the onset of the COVID-19 pandemic.
- Exploratory graphs illustrating trends over time.

---

## Files in This Repository

1. **LA_Crime_Trend_Analysis.Rmd**  
   - The core R Markdown file containing:
     - **Data Loading & Cleaning**: How the dataset is read into R and processed.
     - **Data Categorization**: Labeling crimes as violent, property, or sex crimes.
     - **Statistical Analyses**: Two-sample proportions test and Welch Two-Sample t-test.
     - **Plots & Visualizations**: Time series graphs, bar charts for proportions, etc.  

2. **LA_Crime_Trend_Analysis.html**  
   - The knitted HTML output generated from `LA_Crime_Trend_Analysis.Rmd`.
   - Presents the final, formatted report and findings.

---

## Data Requirements
To replicate the analysis, you will need to download the following datasets (CSV format) from [Data.gov](https://catalog.data.gov/):
1. **Crime Data from 2010 to 2019**  
   [Crime Data from 2010 to 2019](https://catalog.data.gov/dataset/crime-data-from-2010-to-2019)

2. **Crime Data from 2020 to Present**  
   [Crime Data from 2020 to Present](https://catalog.data.gov/dataset/crime-data-from-2020-to-present)

Save them with names like:
- `Crime_Data_from_2010_to_2019.csv`
- `Crime_Data_from_2020_to_present.csv`

Then, update the file paths in the R Markdown code (if necessary) to match where you have stored the CSVs locally.

---

## Usage

1. **Download/Clone the Repository**  
   - Click the green “Code” button in this GitHub repo, then select “Download ZIP” or clone via `git clone https://github.com/yourusername/LA-Crime-Trends-Pre-Post-COVID.git`.

2. **Place the Datasets**  
   - Download the two CSVs (2010–2019 and 2020–present) from the Data.gov links above.
   - Save them in the same folder or adjust the file paths in `LA_Crime_Trend_Analysis.Rmd` as needed.

3. **Install Required R Packages**  
   - This project uses:
     ```r
     install.packages(c("tidyverse", "lubridate", "knitr", "ggplot2", "dplyr"))
     ```
   - Note: If you’re compiling the HTML output, also ensure `rmarkdown` is installed.

4. **Knit the R Markdown**  
   - Open `LA_Crime_Trend_Analysis.Rmd` in RStudio.
   - Click the “Knit” button (choose HTML format).
   - The final knitted HTML report will appear as `LA_Crime_Trend_Analysis.html`.

The `LA_Crime_Trend_Analysis.html` included in this repository is **already** a fully compiled example of what you’ll get if you knit the `.Rmd` file.

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
