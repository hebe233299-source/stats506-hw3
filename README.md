# STATS 506 Homework 3

This project contains the completed R and Quarto analyses for the three problems in [Homework 3](https://phuongov.github.io/stats506-f26/Homework%203/hw03.html): NHANES Poisson models, Sakila SQL/R comparisons, and Australian sample-record processing.

## Files

- `homework3.qmd` — reproducible source with code, tables, figures, and written answers.
- `homework3.html` — executed, self-contained HTML output for Canvas.
- `data/AUX_I.xpt` and `data/DEMO_I.xpt` — original CDC NHANES 2015–2016 XPT files.
- `data/sakila_master.db` — Sakila SQLite database from Bradley Grant's public repository.
- `data/au-500.csv` — Australia 500-record CSV from BrianDunning.com (extracted from the free ZIP).

## Reproduce

Install [R](https://www.r-project.org/) and [Quarto](https://quarto.org/), then install the R packages `haven`, `DBI`, `RSQLite`, `knitr`, and `microbenchmark`. From this directory, run:

```sh
quarto render homework3.qmd --to html
```

The source files are included, so rendering does not download data. Each code chunk runs in document order in a fresh R session. Benchmark times vary by machine and run.

## Sources

- [Official assignment](https://phuongov.github.io/stats506-f26/Homework%203/hw03.html)
- [CDC AUX_I data/codebook](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2015/DataFiles/AUX_I.htm) and [CDC DEMO_I data/codebook](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2015/DataFiles/DEMO_I.htm)
- [Sakila SQLite repository](https://github.com/bradleygrant/sakila-sqlite3)
- [Australian sample-data page](https://www.briandunning.com/sample-data/)

## GitHub submission step

No repository remote is configured in the current workspace. Replace the visible `https://github.com/REPLACE-USERNAME/REPLACE-REPOSITORY` placeholder near the top of `homework3.qmd` with the actual public repository URL, re-render, and upload the resulting HTML to Canvas. Do not submit the placeholder link.
