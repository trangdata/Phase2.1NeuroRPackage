Analysis of COVID-19 patients with Neurological Conditions
================

[![github-action-status](https://img.shields.io/github/workflow/status/trang1618/treeheatr/R-CMD-check?logo=github)](https://github.com/trang1618/treeheatr/actions)

## Install

You can install the development version of **Phase2.1NeuroRPackage**
from GitHub with remotes:

``` r
# install.packages('remotes') # uncomment to install devtools
remotes::install_github('covidclinical/Phase2.1NeuroRPackage')
```

## How to run

The main function `runAnalysis()` has 6 arguments. Please read the
documentation with `?runAnalysis` for a detailed explanation.

``` r
library(Phase2.1NeuroRPackage)

runAnalysis(mysite = 'penn', mask_thres = 10, blur_abs = 0, include_race = TRUE,
            out_dir = 'output', data_dir = '../thrombotic-penn/data')
```

See your site obfuscation parameters (`mask_thres` and `blur_abs`)
[here](https://docs.google.com/spreadsheets/d/1Xl9juDBXt86P3xQtsoTaBl2zPl1BIiAG9DI3Rotyqp8/edit#gid=212461777).
If your site does not have race information, set `include_race = FALSE`.

Please submit the results to the central repository:

``` r
FourCePhase2.1AKI::submitAnalysis()
```

If you run into any problem adapting this code to your data, let us
(@meghutch and @trang1618) know via Slack or [submit an
issue](https://github.com/covidclinical/Phase2.1NeuroRPackage/issues/new).

Thank you very much for your support!
