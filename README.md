# BIS180LTutorials

This repository contains some [learnr]() interactive tutorials for R.

There are currently four tutorials:

* "Tidyverse_Introduction" introduces concepts and tools important for using [tidyverse]() packages.
* "ggplot" teaches basic [ggplot2]() plotting skills
* "Gather_And_Spread" focuses on converting data between long and wide formats
* "Joins" illustrates how to join multiple data frames based on shared keys

## Installing the tutorials

First you need to have `learnr` and `devtools` installed.

From within R:
```
#only needs to be done once per computer
install.packages("learnr")
install.packages("devtools")
```

Then install the tutorials themselves:
```
devtools::install_github("UCDBIS180L/BIS180LTutorials") # only needs to be done once per computer
```

## Starting the tutorials

When you want to actually use the tutorial, then:
```
learnr::run_tutorial("TUTORIAL_NAME", package = "BIS180LTutorials") 
```
where "TUTORIAL_NAME" gets replaced by one of "Tidyverse_Introduction", "ggplot", "Gather_And_Spread", or "Joins".  (keep the quotes).
