
<!-- README.md is generated from README.Rmd. Please edit that file -->

# dhsclogger

dhsclogger provides a convenience wrapper to the family of
`futile.logger` functions to promote use of standardised logging. For
more information see the `futile.logger`
[documentation](https://github.com/zatonovo/futile.logger)

## Installation

You can install the development version of dhsclogger like so:

``` r
remotes::install_github("DataS-DHSC/dhsclogger")
```

## Example usage

To create a log for use in your code:

``` r
library(dhsclogger)

# get logger collection
log <- get_dhsc_logger()

# set threshold of console log to warnings and above
log$set_threshold("log.console", "WARN")

# below will only be printed to the log file
log$info("Script started")
```

## Licence

Unless stated otherwise, the codebase is released under the MIT License.
This covers both the codebase and any sample code in the documentation.
The documentation is © Crown copyright and available under the terms of
the [Open Government 3.0
licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).
