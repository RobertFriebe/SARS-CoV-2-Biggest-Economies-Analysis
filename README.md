# SARS-CoV-2-Biggest-Economies-Analysis
How does the world's biggest economies cope with COVID-19 until April 2020

## Installations
- Python 3, Anaconda3, Jupyter Notebook
- libraries (already present) pandas, numpy, matplotlib.pyplot, seaborn, sklearn

## Motivations

A worldwide monitoring of the course of the pandemic is made possible by the provision of what is probably the most widely used data set at present (Johns Hopkins University: COVID19 dataset). It reports on a daily basis the total number of confirmed infections, recoveries and deaths. This dataset will be used, to answer the questions of how the world’s biggest economies are coping with the pandemic since the day of the outbreak (date from which more than 100 cases were reported).

## Files

### Johns Hopkins COVID-19 Data
#### Confirmed, Recovered, Deaths
- Province/State: Not present for all countries
- Country/Region: 
- Lat: Latitude
- Long: Logitude
- date_1 .... date_n: value of confirmed, recovered, deaths (values are cumulative)

### World Bank Data

#### Population by Country
Timeliness of the population: 2018
- Country Name
- Country Code: Alpha-3 code
- Year: 1960 - 2018
- Value: Number of inhabitants

#### World Bank Region by Income
XLS-File, Register *Data*
- Economy: Country Name
- Code: Alpha-3 code
- Region: World Bank Region (South Asia, Europe & Central Asia, Middle East & North Africa, East Asia & Pacific, Sub-Saharan Africa, Latin America & Caribbean, North America)
- Income Group: High income, upper middle income, lower middle income, low income
- Lending category: not present for all countries (Blend, IBRD, IDA), https://datahelpdesk.worldbank.org/knowledgebase/articles/378834-how-does-the-world-bank-classify-countries 
- Other: not present for all countries (Heavily Indebted Poor Country (HIPC), European Monetary Union (EMU))
