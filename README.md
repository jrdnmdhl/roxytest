
<!-- README.md is generated from README.Rmd. Please edit only README.Rmd! -->

<!-- badges: start -->

[![R build
status](https://github.com/mikldk/roxytest/workflows/R-CMD-check/badge.svg)](https://github.com/mikldk/roxytest/actions)
<!-- badges: end -->

# roxytest

Inline tests with roxygen and testthat.

See demo package using this at
[roxytestdemo](https://github.com/mikldk/roxytestdemo).

## Install

To build and install from Github run this command from within `R`:

    devtools::install_github("mikldk/roxytest", 
                             build_opts = c("--no-resave-data", "--no-manual"))

You can also install the package without vignettes if needed as follows:

    devtools::install_github("mikldk/roxytest")

## Usage

There are a number of roclets included:

  - `testthat_roclet`
  - `tinytest_roclet`
  - `param_roclet`
  - `return_roclet`
  - `examples_roclet`

Please refer to the
“[Introduction](https://mikldk.github.io/roxytest/articles/introduction.html)”
vignette for details on these.

## Notes

  - Rstudio: CTRL+SHIFT+D option does not run `devtools::document()` but
    only `devtools::document(roclets=c('rd', 'collate', 'namespace'))`
    (possibly with fewer, but not none)
      - Use `devtools`’ `document()` addin: see e.g. [Rstudio
        documentation](https://rstudio.github.io/rstudioaddins/), and
        override the keyboard shortcut
