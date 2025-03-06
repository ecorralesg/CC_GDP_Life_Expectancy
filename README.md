# Life Expectancy vs. GDP Analysis

## Overview
This repository contains a data science project exploring the relationship between a country’s Gross Domestic Product (GDP) and its average Life Expectancy. The analysis focuses on six countries (Chile, China, Germany, Mexico, the USA, and Zimbabwe) over the period 2000–2015. Key findings indicate a positive correlation between GDP and Life Expectancy, although the strength and patterns vary by country.

## Contents
1. **Data**  
   - A CSV file (`all_data.csv`) containing the dataset with columns: `['Country', 'Year', 'life_expectancy', 'GDP']`.

2. **Notebooks**  
   - `life_expectancy_gdp.ipynb`: A Jupyter Notebook that walks through data cleaning, descriptive statistics, visualization, and regression analyses (OLS and multiple regression).

3. **README.md** (This file)  
   - Provides an overview of the project.

## Project Setup
1. **Environment**  
   - Python 3.7+  
   - Recommended libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `scipy`

2. **Installation**  
   - Clone this repo:
     ```bash
     git clone https://github.com/ecorralesg/CC_GDP_Life_Expectancy.git
     cd CC_GDP_Life_Expectancy
     ```
   - Create a virtual environment (optional but recommended):
     ```bash
     python -m venv venv
     source venv/bin/activate  # or .\venv\Scripts\activate on Windows
     ```
   - Install the required libraries:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Notebook**  
   - Start Jupyter:
     ```bash
     jupyter notebook
     ```
   - Open `life_expectancy_gdp.ipynb` from your browser and run the cells in order.

## Usage
- **Data Cleaning**  
  The notebook begins by checking for missing or invalid values and ensuring that the dataset is properly formatted (e.g., numeric columns, correct date ranges).
- **Exploratory Data Analysis**  
  Generates descriptive statistics and initial plots (histograms, box plots) to understand distributions and outliers.
- **Advanced Analysis**  
  - _Year-to-year comparisons_ of GDP and Life Expectancy.  
  - _Simple regressions per country_.  
  - _ANOVA tests_ for average Life Expectancy differences among countries.  
  - _Multiple regression_ including GDP, Year, and Country effects.
- **Visualizations**  
  - **Violin Plot**: Shows the distribution of Life Expectancy by country.  
  - **Facet Grid Scatter**: GDP vs. Life Expectancy for each country in separate panels.  
  - **Facet Grid Line**: GDP by year and Life Expectancy by year in separate subplots.

## Key Findings
1. **Positive Correlation**  
   Generally, higher GDP correlates with higher Life Expectancy.
2. **Country-Specific Slopes**  
   Different countries show different rates of change and baseline levels.
3. **Time Trend**  
   Over 2000–2015, nearly all countries experienced increased Life Expectancy and growing GDP.
4. **Statistical Significance**  
   Multiple regression suggests GDP remains a significant factor even when controlling for time trends and country-level differences.

## Limitations and Future Work
- **Limited Years**  
  The dataset covers only 16 years, potentially missing longer-term patterns.
- **Economic Metrics**  
  GDP alone doesn’t capture income inequality or how wealth is distributed.
- **Other Factors**  
  Life Expectancy is influenced by healthcare systems, environment, education, etc.
  Future work could incorporate these additional variables for a more robust model.
