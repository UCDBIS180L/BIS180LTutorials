# BIS180LTutorials

This repository contains some [learnr](https://rstudio.github.io/learnr/) interactive tutorials for R.

There are currently four tutorials:

* "Tidyverse_Introduction" introduces concepts and tools important for using [tidyverse](https://www.tidyverse.org/) packages.
* "ggplot" teaches basic [ggplot2](https://ggplot2.tidyverse.org/) plotting skills
* "Gather_And_Spread" focuses on converting data between long and wide formats (deprecated, use Pivot)
* "Pivot" focuses on converting data between long and wide formats
* "Joins" illustrates how to join multiple data frames based on shared keys
* "Stringr_and_Regex" Introduced regular expressions and string manipulation with the stringr package.


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

## Additional resources

The material introduced in these tutorials is covered in much more detail in [R for data science](http://r4ds.had.co.nz/) by Garrett Grolemund and Hadley Wickham

## Serving the tutorials

If you want to serve the tutorials on a shiny server instance, then:

* be sure that the directory containing the tutorials is owned by shiny
* delete the .html file associated with each tutorial

