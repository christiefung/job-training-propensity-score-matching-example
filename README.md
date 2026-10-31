# Propensity Score Methods: A Job-Training Program Example

A short, reproducible R analysis showing a policy-evaluation workflow with observational data.

**Question:** Did participation in a job-training program raise 1978 earnings?

**Data:** the `lalonde` dataset included in the [`MatchIt`](https://kosukeimai.github.io/MatchIt/) R package (public, no download needed).

## What it demonstrates

- Defining the estimand (ATT)
- Checking covariate balance and propensity score overlap
- Estimating the effect with matching and with weighting
- Comparing methods to see how much the answer depends on the specification
- Stating limitations, including unobserved confounding

## Run it

```r
install.packages(c("MatchIt", "cobalt", "dplyr", "ggplot2", "sandwich", "lmtest", "rmarkdown"))
rmarkdown::render("analysis.Rmd")
```

This produces `analysis.html` with all tables and figures.

## Files

- `analysis.Rmd`: full analysis (code, output and interpretation)
- `README.md`: this file

## Note

This is a methods illustration on a well-known public dataset, not a new evaluation of the original program.

Author: Ka Man (Christie) Fung
