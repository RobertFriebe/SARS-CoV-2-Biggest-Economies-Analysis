# SARS-CoV-2-Biggest-Economies-Analysis
How does the world's biggest economies cope with COVID-19 until April 2020

## 1. Installations
- Python 3, Anaconda3, Jupyter Notebook
- libraries (already present) pandas, numpy, matplotlib.pyplot, seaborn, sklearn

## 2. Motivations

A worldwide monitoring of the course of the pandemic is made possible by the provision of what is probably the most widely used data set at present (Johns Hopkins University: COVID19 dataset). It reports on a daily basis the total number of confirmed infections, recoveries and deaths. This dataset will be used, to answer the questions of how the world’s biggest economies are coping with the pandemic since the day of the outbreak (date from which more than 100 cases were reported).

## 3. Files

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

#### Final_Dataset 
Used for Analysis (SARS-CoV-2-Biggest-Economies-Analysis.ipynb)
- Country/Region
- Code: Alpha-3 code
- Region: World Bank Region
- Income Group: High income, upper middle income, lower middle income, low income
- Population: year 2018
- Date: End of January to Begining of May 2020
- Days_since_outbreak: Counter for number of days on which more than 100 cases are confirmed in a country region
- confirmed: cumulative
- recovered: cumulative
- deaths: cumulative
- confirmed_new: Change of confirmed current date - confirmed previous date
- recovered_new: Change of recovered current date - recovered previous date
- deaths_new: Change of deaths current date - deaths previous date
- active: confirmed - recovered
- active_new: active current - active previous
- v_t_clean_5ma: Daily Doubling time, 5 day moving average
- confirmed_100k: Confirmed cases by 100.000 inhabitants = confirmed / (population / 100000)
- perc_infected_dn: Infestation Rate = Percentage of already infected persons under consideration of unreported cases
- perc_cfr_dn: Case-related Fatality Rate under consideration of unreported cases
- confirmed_dn: confirmed cases under consideration of unreported cases
- cfr: case fatality rate (https://www.thelancet.com/journals/laninf/article/PIIS1473-3099(20)30246-2/fulltext)
- cmr: crude mortality rate (http://www.gbe-bund.de/gbe10/abrechnung.prc_abr_test_logon?p_uid=gast&p_aid=0&p_knoten=FID&p_sprache=E&p_suchstring=10099::Mortality%20figures)


# 4. How to interact with the data
- There is a final-dataset for analysis that can be use for own analyses
- There is also an option to use the jupyter notebook and download the lates JHU-COVID19 date from the repositry, wrangle the date and create an up-do-date dataset for analyses

# 5. Authors and others
- Analysis made by Robert Friebe, May 2020
Data-Ressources as follows:
- World Bank Regions: https://datahelpdesk.worldbank.org/knowledgebase/articles/906519-world-bank-country-and-lending-groups
- Population by Country (Up-to-dateness: 2018): https://github.com/datasets/population/tree/master/data
- JHU-SARS-CoV-2 data: https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series
