[![Travis-CI Build Status](https://travis-ci.org/reconhub/outbreaks.svg?branch=master)](https://travis-ci.org/reconhub/outbreaks)
[![Build status](https://ci.appveyor.com/api/projects/status/62gcky08onmr69x8/branch/master?svg=true)](https://ci.appveyor.com/project/thibautjombart/outbreaks/branch/master)
[![CRAN_Status_Badge](https://www.r-pkg.org/badges/version/outbreaks)](https://cran.r-project.org/package=outbreaks)
[![CRAN Downloads](https://cranlogs.r-pkg.org/badges/outbreaks)](https://cran.r-project.org/package=outbreaks)
[![Downloads from Rstudio mirror](https://cranlogs.r-pkg.org/badges/grand-total/outbreaks)](https://www.r-pkg.org/pkg/outbreaks)

<br>

# outbreaks: a compilation of disease outbreak data

This package compiles a series of publicly available disease outbreak data.
Data can be provided as R objects (loaded automatically when loading the package), text files distributed alongside the package, or functions generating a dataset.

The following R datasets are currently available:



```r
data(package="outbreaks")
```



Table: Data sets in outbreaks

|Item                             |Title                                                                           |
|:--------------------------------|:-------------------------------------------------------------------------------|
|covid19_england_nhscalls_2020    |Potential COVID19 cases reported through NHS pathways                           |
|dengue_fais_2011                 |Dengue on the island of Fais, Micronesia, 2011                                  |
|dengue_yap_2011                  |Dengue on the Yap Main Islands, Micronesia, 2011                                |
|ebola_kikwit_1995                |Ebola in Kikwit, Democratic Republic of the Congo, 1995                         |
|ebola_sierraleone_2014           |Ebola in Sierra Leone, 2014                                                     |
|ebola_sim                        |Simulated Ebola outbreak                                                        |
|ebola_sim_clean                  |Simulated Ebola outbreak                                                        |
|fluH7N9_china_2013               |Influenza A H7N9 in China, 2013                                                 |
|influenza_england_1978_school    |Influenza in a boarding school in England, 1978                                 |
|measles_hagelloch_1861           |Measles in Hagelloch, Germany, 1861                                             |
|mers_korea_2015                  |Middle East respiratory syndrome in South Korea, 2015                           |
|nipah_malaysia                   |Nipah in Malaysia and Sinagapore, 1997-1999                                     |
|norovirus_derbyshire_2001_school |Norovirus in a primary school in Derbyshire, England, 2001                      |
|rabies_car_2003                  |Dog Rabies in Central African Republic, 2003-2012                               |
|s_enteritidis_pt59               |Salmonella Enteritidis PT59 outbreak                                            |
|sars_canada_2003                 |Severe Acute Respiratory Syndrome in Canada, 2003                               |
|sarscov2_who_2019                |SARS-CoV-2 World Health Organization Situation Reports 2019 Outbreak (COVID-19) |
|smallpox_abakaliki_1967          |Smallpox in Abakaliki, Nigeria, 1967                                            |
|varicella_sim_berlin             |Simulated Varicella outbreak                                                    |
|zika_girardot_2015               |Zika in Girardot, Colombia, 2015                                                |
|zika_sanandres_2015              |Zika in San Andres, Colombia, 2015                                              |
|zika_yap_2007                    |Zika on the Yap Main Islands, Micronesia, 2007                                  |


<br>

# Installing the package

To install the current stable, CRAN version of the package, type:

```r
install.packages("outbreaks")
```

To benefit from the latest features and bug fixes, install the development, *github* version of the package using:

```r
devtools::install_github("reconhub/outbreaks")
```

Note that this requires the package *devtools* installed.



<br>

## Add your own data!

### How to add data?
We will try to create a better repository and data submission system at a later stage.
The purpose of the current package is only to share examplar datasets during the hackathon.
Acceptable forms are:
- as a `.RData` files in the `data/` folder (recommended)
- as a text file in the `inst/` folder
- as a function loading/assembling/simulating a dataset

### Naming Conventions
We use the lower case throughout, and snake_case (using underscores) to separate words for the files and dataset names, so that for a `RData` object, a new dataset woud look like: `my_new_data_RData'. Try using informative names, typically using the disease first. Whenever available, order fields as:
   1. *disease*: mandatory
   2. *location*: optional
   3. *year*: optional
   4. *sim*: mandatory if this is a simulated dataset; otherwise data is assume to be an actual outbreak
   5. *other*: (any other relevant information)


<br>

### Contributors (by alphabetic order):
- [Eric Brown](https://github.com/eebrown)
- [Finlay Campbell](https://github.com/finlaycampbell)
- [Simon Frost](https://github.com/sdwfrost)
- [Thibaut Jombart](https://github.com/thibautjombart)
- Pierre Nouvellet
- Sang Woo Park
- [Juliet R.C. Pulliam](https://github.com/jrcpulliam)
- [Jakob Schumacher](https://github.com/jakobschumacher)
- Bertrand Sudre

Maintainer: Finlay Campbell (finlaycampbell93@gmail.com)
