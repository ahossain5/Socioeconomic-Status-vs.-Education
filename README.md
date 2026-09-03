# Socioeconomic Status vs. Education


## Project Overview

This project analyzes the relationship between socioeconomic conditions and educational attainment across U.S. counties using county-level data from the USDA Economic Research Service (ERS).

The analysis examines median household income, poverty rates, and educational attainment to explore how socioeconomic conditions relate to education across different areas of the United States.

The purpose of this project was to demonstrate how raw data can be transformed into a clear story through proper analysis and visualization. The datasets were organized around a shared field, allowing information from each dataset to be connected and analyzed together. Using Excel Power Pivot, I built relationships between the datasets and developed PivotTables and charts to examine trends and comparisons. The analysis was then expanded into an interactive Power BI dashboard to present key findings in a clear and accessible way.


## Data Sources

The data used in this project was obtained from the USDA Economic Research Service (ERS) and includes county-level information on poverty, median household income, and educational attainment. These datasets were downloaded directly from the USDA ERS County-level Data Sets page and are available in Excel format.

**Source:**  [USDA Economic Research Service – County-level Data Sets](https://www.ers.usda.gov/data-products/county-level-data-sets/county-level-data-sets-download-data)

**Project Data:** [View Raw Data Files](./Raw%20Data/)


## Data Preparation

The data preparation process began with multiple Excel datasets downloaded from the USDA Economic Research Service (ERS). The files were reviewed and cleaned before being consolidated into a single Excel workbook for further analysis.

Since the datasets contained different measured, I used the FIPS code as the common field to ensure that each county was represented consistently across the data. I reviewed and aligned the FIPS codes across all four datasets, resulting in 3,186 matching records in each dataset.

Once the data was cleaned and aligned, the prepared datasets were organized into a single Excel workbook for use in the Power Pivot data model and subsequent analysis.


## Excel & Power Pivot Analysis

After preparing the data, I used Excel Power Pivot to build a relational data model connecting the datasets through their shared FIPS codes. This allowed fields from multiple tables to be used together while keeping each dataset organized separately.

Using the completed data model, I created three PivotTables to explore the relationships between socioeconomic status and educational attainment. Each PivotTable was designed to answer a different question within the analysis and was paired with a chart to make the results easier to interpret.

### PivotTable 1 – Median Household Income vs. Poverty Rate

The first PivotTable examines the relationship between median household income and poverty rates across counties within a selected state. Georgia was selected as an example to provide a more focused and readable comparison, although the PivotTable can be filtered to any state.

Conditional formatting was applied to highlight counties that fell below Georgia's average median household income and counties with poverty rates below the state average. Comparing the highlighted values across both measures revealed an inverse pattern between poverty and income, with lower poverty rates generally associated with higher median household incomes.

### PivotTable 2 – Educational Attainment vs. Median Household Income

The second PivotTable examines the relationship between educational attainment and median household income across counties within a selected state. Georgia was again selected as an example to provide a more focused and readable comparison, although the PivotTable can be filtered to any state.

The counties were sorted from lowest to highest based on the number of adults with a bachelor's degree or higher, making it easier to observe how median household income changes alongside educational attainment. The comparison revealed a generally positive relationship, with higher levels of educational attainment often associated with higher median household incomes.

### PivotTable 3 – Poverty vs. Educational Attainment

The third PivotTable examines the relationship between poverty and lower levels of educational attainment across counties. Filtering was used to narrow the data and allow specific areas to be examined more closely.

The analysis compares the population living in poverty with the number of adults who did not graduate from high school. A scatter plot was created from the PivotTable to visualize the relationship between these two measures, with a trendline added to help identify the overall pattern.

The chart shows a strong positive relationship, with counties that have larger populations of adults without a high school diploma also tending to have larger populations living in poverty. The trendline produced an R² value of 0.9974, indicating that the two measures closely follow the observed linear pattern within this analysis.

However, both measures represent population counts rather than rates, meaning county population size may influence the strength of this relationship. The result should therefore be interpreted as an observed association between the two measures rather than evidence that lower educational attainment directly causes higher poverty.

## Power BI Dashboard

After completing the Excel and Power Pivot analysis, I used Power BI to bring the key findings together into a single interactive dashboard. The dashboard provides a broader view of educational attainment, poverty, and median household income while allowing socioeconomic patterns to be compared across states.

The visualizations were designed to present the findings from multiple perspectives, making it easier to identify overall patterns and compare socioeconomic and educational measures across different areas of the United States.

![Power BI Dashboard](./Power%20BI/Dashboard%20(Socioeconomic%20Status%20vs.%20Education).png)


## Key Findings

- **Income and Poverty:** Counties with lower poverty rates generally had higher median household incomes, showing an inverse relationship between the two measures.

- **Education and Income:** Counties with higher levels of educational attainment generally tended to have higher median household incomes, indicating a positive relationship between education and income.

- **Education and Poverty:** Counties with larger populations of adults without a high school diploma also tended to have larger populations living in poverty. Because both measures are population counts, county size may contribute to the strength of this relationship.


## Tools & Skills

- **Microsoft Excel** – Data cleaning, organization, PivotTables, conditional formatting, sorting, filtering, and chart creation
- **Power Pivot** – Relational data modeling and creating relationships between multiple datasets using shared fields
- **Power BI** – Interactive dashboard development and data visualization
- **Data Preparation** – Combining multiple datasets, aligning records, and preparing data for analysis
- **Data Analysis** – Identifying, comparing, and interpreting relationships between socioeconomic and educational measures
- **Data Visualization** – Communicating findings through charts, scatter plots, trendlines, and interactive visuals


## Repository Structure

The repository is organized to reflect the progression of the project from raw data to final analysis and visualization.

- **[Raw Data](./Raw%20Data/)** – Original Excel datasets downloaded from the USDA Economic Research Service (ERS)
- **[Cleaned Data](./Cleaned%20Data/)** – Prepared and aligned datasets used for analysis
- **[Excel Analysis](./Excel%20Analysis/)** – Excel workbook containing the Power Pivot data model, PivotTables, and charts
- **[Power BI](./Power%20BI/)** – Power BI project file and dashboard preview



