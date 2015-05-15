shinyapps
=======================================================

An R package used for deploying applications to the
[ShinyApps](http://shinyapps.io/) hosted service. See
[how this fork differs from upstream](#this-fork).

ShinyApps is not yet generally available however if you are interested in alpha
or beta testing the service you can sign up here: http://shinyapps.io/

## Installation

To install directly from GitHub, run this:

```
if (!require("devtools"))
    install.packages("devtools")
devtools::install_github("dlukes/shinyapps")
```

## Usage

To get started using ShinyApps checkout the
[Getting Started Guide](https://github.com/rstudio/shinyapps/blob/master/guide/guide.md).

## <a name="this-fork"></a>This fork

This fork differs only by adding `bundleApp()` to the list of functions
exported by the NAMESPACE, making it easy to create a gzipped tarball of a
Shiny app locally and then deploy it manually to a custom server instead of
https://shinyapps.io.
