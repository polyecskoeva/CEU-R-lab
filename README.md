This is the R script repository of the "[Tools for Analytics Lab - R-track](http://economics.ceu.edu/courses/1-tools-analytics-lab-r-track)" course, part of the [MSc in Business Analytics](http://business.ceu.edu/msc-in-business-analytics) at CEU.

### Jan 25 (90 min): Introduction to R and General Programming

* General overview of the R ecosystem: [slides](http://bit.ly/CEU-R-1)
* Introduction to R: [variables, functions and vectors](https://github.com/daroczig/CEU-R-lab/blob/master/1.R)

### Jan 26 (90 min): First Steps with Data Visualization

* Review of the most important R object types
* Quick overview of the missed `data.frame` examples from yesterday
* Exploratory data analysis with the most often used plots
* Plots outside of Excel: `dotchart` and `vioplot` examples
* The Grammar of Graphics in R with `ggplot2`

### Jan 27 (140 min): Data Preparation

* [GitHub registration](https://github.com/join)

* `ggplot2` exercises
    * number of carburetors
    * horsepower
    * barplot of number of carburetors per transmission
    * boxplot of horsepower by the number of carburetors
    * horsepower and weight by the number of carburetors
    * horsepower and weight by the number of carburetors with a trend line

* Filtering and summarizing data with base `R`
* Intro to `data.table`
* `data.table` exercises with `hflights`
    * the number of cancelled flights
    * the shortest flight on each weekday
    * the average delay to all destination
    * the average delay to all destination per destination
    * plot the departure and arrival delays
    * plot the average departure and arrival delays per destination
    * plot the average departure and arrival delays per flight + size
    * estimate the delay to Budapest

* Some quick examples on string and date manipulations
* Left joins

### Jan 28 (140 min): Models

* Revisiting GitHub integration in RStudio:
    1. Install git from https://git-scm.com/
    2. Install R from https://www.r-project.org/
    3. Install RStudio from https://www.rstudio.com/products/RStudio/#Desktop
    4. Verify that in RStudio, you can see the path of the `git` executable binary in the Tools/Global Options menu's "Git/Svn" tab -- if not, then you might have to restart RStudio (if you installed git after starting RStudio) or installed git by not adding that to the PATH on Windows. Either way, browse the "git executable" manually (in some `bin` folder look for thee `git` executable file).
	5. Create an RSA key (optionally with a passphrase for increased security -- that you have to enter every time you push and pull to and from GitHub). Copy the public key and add that to you SSH keys on your GitHub profile.
    6. Create a new project choosing "version control", then "git" and paste the SSH version of the repo URL copied from GitHub in the pop-up -- now RStudio should be able to download the repo. If it asks you to accept GitHub's fingerprint, say "Yes".
    7. If RStudio/git is complaining that you have to set your identity, click on the "Git" tab in the top-right panel, then click on the Gear icon and then "Shell" -- here you can set your username and e-mail address in the command line, so that RStudio/git integration can work. Use the following commands:

	    ```
        $ git config --global user.name "Your Name"
        $ git config --global user.email "Your e-mail address"
		```
		
		Close this window, commit, push changes, all set.
		
* Correlation, causality
* Linear regression
* Goodness of fit
* Polynomial regression
* Overfitting
* Confounders

Datasets and references for the model examples:
* [height & weight dataset](http://bit.ly/BudapestBI-R-csv)
* [OLS trend line distance from actual points](http://psycho.unideb.hu/statisztika/pages/interaktiv.html)
* [Shoe size & math](http://bit.ly/math_and_shoes)
* [Bickel et al 1975](http://bit.ly/bickel-1975)