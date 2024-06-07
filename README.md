# NORS National Outbreak Data Analysis and Visualization

## Overview

This project analyzes and visualizes national outbreak data from the CDC's National Outbreak Reporting System (NORS). The analysis focuses on foodborne outbreaks in the United States from 2011 to 2021. The final report includes data aggregation, a Poisson regression model, and mapping of outbreak prevalence.

## Project Structure

The project contains the following key components:

- `Final_Data.Rmd`: The R Markdown file containing the full analysis and visualization code.
- `Final_Data.html`: The rendered HTML report of the analysis.
- `NationalOutbreakPublicDataTool.xlsx`: The dataset downloaded from the CDC NORS website.
- `States_shapefile.*`: Shapefiles used for mapping the outbreak data.

## Data Retrieval

1. Visit the [CDC NORS website](https://wwwn.cdc.gov/norsdashboard/).
2. Check only the "Foodborne" box for type of outbreak.
3. Under "Year" select "Custom range" and input from 2011 to 2021 (10 years).
4. Scroll down to "Download Data" and click "Download current search data (excel)" to import the data on your local machine.
5. Save the downloaded Excel file as `NationalOutbreakPublicDataTool.xlsx` in the project directory.

## Poisson GLM
The data is aggregated by state and year, and a Poisson regression model is fitted to analyze the total number of illnesses.

## Mapping Outbreak Prevalence
The aggregated data is merged with state shapefiles to visualize the prevalence of foodborne illnesses.

## How to Run the Analysis
1. Ensure all necessary files (`Final_Data.Rmd`, `NationalOutbreakPublicDataTool.xlsx`, and shapefiles) are in the project directory.
2. Open `Final_Data.Rmd` in R Studio.
3. Knit the document to produce `Final_Data.html`.

## Final Report
To review the final report, please refer to Final_Data.html.
