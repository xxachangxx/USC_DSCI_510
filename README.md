## Introduction

The project is for USC DSCI 510

dir ./data contains raw data and data for analysis

dir ./code contains code for fetching data and analysis

## **What data did you collect**

* General Nature: COVID-19 Statistic
* **Data Source**: 
  1.  [Data from github](https://github.com/owid/covid-19-data/tree/master/public/data): use `wget` to fetching the data 
      * [raw data](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/owid-covid-data.csv)
      * [code book](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/owid-covid-data.csv)
  2.  [VACCOVID API](https://vaccovid-coronavirus-vaccine-and-treatment-tracker.p.rapidapi.com/api/npm-covid-data/): use python requests to get the data

### update

#### 11/30/2022

* Because of **523 Server Error**, the VACCOVID is temporarily unreachable, I will download it once it get recovered. If it cannot recover, I wil discard it and only use data from github/owid/covid-19-data.git

* Data from github is from multiple sources. I guess it could meet the Homework need for "2 or more sources"

  > * Confirmed cases and deaths:our data comes from theCOVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University(JHU). We discuss how and when JHU collects and publishes this data here. The cases & deaths dataset is updated daily.
  >
  > - Note: confirmed cases and deaths are collected by Johns Hopkins University by date of report, rathen than date of test/death. Therefore the number they report on a given day does not necessarily represent the actual number on that date, because of the long reporting chain that exists between a new case/death and its inclusion in statistics. This also means that time series can show sudden changes (negative or positive) when a country corrects historical data, because it had previously under- or overestimated the number of cases/deaths.
  >
  > - **Hospitalizations and intensive care unit (ICU) admissions:** our data is collected from official sources and collated by Our World in Data. The complete list of country-by-country sources is available [here](https://github.com/owid/covid-19-data/blob/master/public/data/hospitalizations/locations.csv).
  > - **Testing for COVID-19:** this data is collected by the *Our World in Data* team from official reports; you can find further details in our post on COVID-19 testing, including our [checklist of questions to understand testing data](https://ourworldindata.org/coronavirus-testing#our-checklist-for-covid-19-testing-data), information on [geographical and temporal coverage](https://ourworldindata.org/coronavirus-testing#which-countries-do-we-have-testing-data-for), and [detailed country-by-country source information](https://ourworldindata.org/coronavirus-testing#source-information-country-by-country). **On 23 June 2022, we stopped adding new datapoints to our COVID-19 testing dataset.** You can read more [here](https://github.com/owid/covid-19-data/discussions/2667).
  > - **Vaccinations against COVID-19:** this data is collected by the *Our World in Data* team from official reports.
  > - **Other variables:** this data is collected from a variety of sources (United Nations, World Bank, Global Burden of Disease, Blavatnik School of Government, etc.). More information is available in [our codebook](https://github.com/owid/covid-19-data/tree/master/public/data/owid-covid-codebook.csv).