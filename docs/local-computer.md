# Running STRAF on a local computer {#local-computer}

## Intro

STRAF is a web application, using the Shiny web application framework, based 
on the R programming language. It has been designed to work with a web browser
and typically runs on a distant server.

There are several reasons for which one would prefer not using an application
hosted on a web server: restrictions around the use of data, 
limited computational resources on the server, ...

In this chapter, we describe a way to run STRAF on a local computer. It requires 
to install some dependencies (in particular, R and the straf R package) to be
able to run STRAF locally.

## Prerequisites

### Installing R

You first need to install R, the language in which STRAF is programmed. 

1. If your system is running under __Windows__, you can follow [this link](http://cran.r-project.org/bin/windows/base/). You can download the 
installation software from there and then follow the
instructions to install R on your system.

2. If your system is running under __Mac OS__, follow [this link to install R](http://cran.r-project.org/bin/macosx/)

3. Finally, if you are using a __Linux__ system,you should be able to install R 
using the using the following commands:

```
sudo apt update
sudo apt -y upgrade
sudo apt -y install r-base
```

Now, you should be able to run R-based software like STRAF on your computer.

### Installing RStudio

__RStudio__ is a free an open-source user-friendly environment built on top of R, that
you can download from [this website](https://www.rstudio.com/products/rstudio/download).


### Install the shiny and straf packages

Now you can __open RStudio__ and copy, paste and run the following __commands__ in the
R Console:

```
install.packages("remotes")
remotes::install_github("agouy/straf")
```

Now, the `straf` R package should be installed on your system, which means you
are now able to run the app on your personal computer. You won't need to re-run
the previous commands now that the package is present on your system.

## Launching the application

You can now launch the application by copying and pasting the following commands 
in the console:

```
library(straf)
runStraf()
```

_Et voilà!_ You should now have an open window. STRAF is running on your local 
computer, even though it uses a web browser, so the data you "upload" this way 
would in practice remain on your computer.
