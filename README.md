# Correlation between Inflation and Unemployment

## Overview
This project investigates the relationship between inflation and unemployment using data from FRED and the World Bank.
We test for correlation and estimate a simple linear model (Phillips-curve style) using monthly U.S. data and
annual international data.

##Files and Roles
###data/ — datasets used in the project
1.T10YIE.csv — 10-Year Breakeven Inflation Rate (FRED)
2.UNRATE.csv — Unemployment Rate (FRED)
3.API_FP.CPI.TOTL.ZG_DS2_en_csv_v2_130173.csv — World Bank inflation (consumer prices, %)
4.API_SL.UEM.TOTL.NE.ZS_DS2_en_csv_v2_125709.csv — World Bank unemployment (% of labor force)

###Scripts/ — code organization
00_requirements.R — installs/loads required packages (tidyverse, lubridate, broom, ggplot2)
01_data_load.R — reads and cleans the datasets; aligns date/years
11_Breakev_Inf_By_Unem.R — analysis & plots for FRED (breakeven inflation vs. unemployment)
12_CPI_By_Unem.R — analysis & plots for World Bank (CPI vs. unemployment)

###Rmd’s
FinalReport.Rmd — combines all text, code, and figures into a complete reproducible report.


###report
FinalReport.pdf — final rendered report from the Rmd file, showing code output, analysis, and written interpretation.


##Reproducibility Instructions
1. Open the project file `FinalProject.Rproj` in RStudio.  
2. Run `Scripts/00_requirements.R` to load all packages.  
3. Knit `FinalReport.Rmd` to generate the final report (`FinalReport.pdf`).  
4. All data paths are relative, so the project can be run on any computer as long as 
the `data/` folder is in the same directory.