[![Travis-CI Build Status](https://travis-ci.org/reconhub/outbreaks.svg?branch=master)](https://travis-ci.org/reconhub/outbreaks)

# outbreaks: a compilation of disease outbreak data

This package compiles a series of disease outbreak data, to be shared during Hackout 3.
Data can be provided as R objects (loaded automatically when loading the package), text files distributed alongside the package, or functions generating a dataset.

The following R datasets are currently available:



```r
data(package="outbreaks")
```



|Item                          |Title                                                   |
|:-----------------------------|:-------------------------------------------------------|
|ebola.kikwit.1995             |Ebola in Kikwit, Democratic Republic of the Congo, 1995 |
|ebola.sim                     |Simulated Ebola outbreak                                |
|ebola.sim.clean               |Simulated Ebola outbreak                                |
|fluH7N9.china.2013            |Influenza A H7N9 outbreak in China                      |
|influenza.england.1978.school |Influenza in a boarding school in England, 1978         |
|measles.hagelloch.1861        |Measles in Hagelloch, Germany, 1861                     |
|sars.canada.2003              |Severe Acute Respiratory Syndrome in Canada, 2003       |
|smallpox.abakaliki.1967       |Smallpox cases in Abakaliki, Nigeria in 1967            |

# Installing the package

To install the devel version of the package, type:

```r
devtools::install_github("reconhub/outbreaks")
```

Note that this requires the package *devtools* installed.




## Add your own data!

### How to add data?
We will try to create a better repository and data submission system at a later stage.
The purpose of the current package is only to share examplar datasets during the hackathon. 
Acceptable forms are:
- as a `.RData` files in the `data/` folder (recommended)
- as a text file in the `inst/` folder
- as a function loading/assembling/simulating a dataset

### Naming Conventions
We use the lower cases and dots to separate words for the files and dataset names, so that for a `RData` object, a new dataset woud look like: `my.new.data.RData'. Try using informative names, typically using the disease first. Whenever available, order fields as:
   1. *disease*: mandatory
   2. *location*: optional
   3. *year*: optional
   4. *sim*: mandatory if this is a simulated dataset; otherwise data is assume to be an actual outbreak
   5. *other*: (any other relevant information)


### Contributors (by alphabetic order):
- Finlay Campbell (@finlaycampbell)
- Simon Frost (@sdwfrost)
- Thibaut Jombart (@thibautjombart)
- Pierre Nouvellet


Maintainer: Finlay Campbell (f.campbell15@imperial.ac.uk)
