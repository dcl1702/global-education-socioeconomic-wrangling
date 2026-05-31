# Global Education, Literacy, and Socioeconomic Indicators Analysis

## Overview

This project is an end-to-end data wrangling and analysis project that combines multiple data sources to explore relationships between national socioeconomic indicators, university presence, and literacy rates across countries.

The project uses a flat file, a public API, and a scraped website table. After cleaning and standardizing the data, the datasets are loaded into SQLite, joined into one integrated dataset, and used for visual analysis.

## Objective

The goal of this project was to practice collecting, cleaning, transforming, integrating, and analyzing data from multiple source types.

The analysis focuses on questions such as:

- How do literacy rates relate to GDP per capita?
- How does university availability compare across countries?
- Are education-related indicators connected with broader socioeconomic indicators?
- What patterns appear when country-level data is combined from different sources?

## Data Sources

This project uses three data sources:

1. Global Country Information Dataset 2023  
   A flat file from Kaggle containing country-level socioeconomic indicators such as GDP, population, fertility rate, unemployment, life expectancy, land area, and more.

2. University Domains API  
   A public API containing university names, domains, web pages, and country information.

3. List of Countries by Literacy Rate  
   A Wikipedia table containing literacy rates by country, including youth, adult, and elderly literacy rates.

## Project Files

- `milestone_1_project_plan.docx`: Project plan, data source summary, expected relationships, and ethical considerations
- `milestone_2_flat_file_cleaning.ipynb`: Cleaning and transformation of the country socioeconomic flat file
- `milestone_3_literacy_web_scraping.ipynb`: Web scraping and cleaning of the literacy rate table
- `milestone_4_university_api_cleaning.ipynb`: API collection and cleaning of university domain data
- `milestone_5_database_join_analysis.ipynb`: SQLite loading, table joins, and final visual analysis
- `README.md`: Project documentation
- `requirements.txt`: Python package requirements


## Methods Used

- Flat file data cleaning
- Column name standardization
- Data type conversion
- Web scraping with BeautifulSoup
- API data retrieval with requests
- Country name standardization
- Aggregation of university counts by country
- SQLite database loading
- SQL table joins
- Data visualization with seaborn and matplotlib

## Key Visualizations

The final analysis includes visualizations such as:

- GDP per capita vs adult literacy
- Fertility rate vs youth literacy
- Life expectancy vs adult literacy
- University density per million people vs adult literacy
- Top countries by university count with literacy overlay

## Key Findings

- Many countries have high adult literacy rates, but lower-GDP countries show more variation.
- Countries with higher fertility rates tend to show lower youth literacy rates.
- Countries with higher life expectancy generally also show higher adult literacy rates.
- University density alone does not fully explain literacy outcomes.
- Some countries have many universities but lower literacy rates, suggesting that national-level education outcomes are influenced by more than just institution count.

## Tools Used

- Python
- pandas
- BeautifulSoup
- requests
- SQLite
- matplotlib
- seaborn

## Key Skills Demonstrated

- Multi-source data collection
- Data cleaning and transformation
- Web scraping
- API integration
- Data aggregation
- Relational database loading
- SQL joins
- Exploratory data analysis
- Data visualization
- Ethical consideration of data limitations

## Limitations

The analysis relies on country-level data, which can hide regional and demographic differences within countries. The university API may underrepresent institutions without a strong online presence. Literacy data may also vary in quality, reporting year, and methodology across countries.

## Future Improvements

- Improve country name matching with ISO country codes
- Add more recent literacy and education indicators
- Expand the database schema instead of relying only on one joined table
