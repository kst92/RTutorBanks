This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

This problem set is based on the content of the paper "How Important are Banks for Development? National Banks in the United States, 1870-1900" written by Scott L.Fullford (December 2015). 
Its aim is to investigate if national banks had an effect on the production per person in the United States. The interactive structure of the problemset together with descriptions of economic theory and explanations of R commands grant a diversified and informative journey through the topic.

The paper can be found online at https://www.mitpressjournals.org/doi/pdf/10.1162/REST_a_00546.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
if (!require(devtools))
  install.packages("devtools")
source_gist("gist.github.com/skranz/fad6062e5462c9d0efe4")
install.rtutor(update.github=TRUE)

devtools::install_github("kst92/RTutorBanks", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorBanks)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorBanks")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorBanks",
       load.sav=TRUE, sample.solution=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
