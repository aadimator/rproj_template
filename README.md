# {Project Name}

<p align="center">
    <em>{Project Abstract}</em>
</p>

## Project Description

{Project Description}

## Environment Setup


For R, we will use the `renv` package to manage the environment. The `renv.lock` file contains the necessary packages for R.

To restore the R environment, run the following command:

```R
renv::restore()
```

When you run the `renv::restore()` command, it will create a new environment with the necessary packages. You can activate the environment by running the following command:

```R
renv::activate()
```

Furthermore, running R console from the project root directory will automatically activate the environment.

To install the necessary packages, run the following command:

```R
renv::install("package_name")
```

To save the environment, run the following command:

```R
renv::snapshot()
```

This will update the `renv.lock` file with the new packages.


## Project Organization

```
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for processing.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- Data dictionaries, manuals, and all other explanatory materials.
│
├── notebooks          <- Jupyter or Quarto notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `01-adm-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for pdac_nac
│                         and configuration for tools like ruff.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── renv.lock          <- The requirements file for reproducing the analysis environment.
│
└── src                <- Source code for use in this project.
    │
    └── pipeline       <- Folders for different stages of the pipeline
        └── visualize.R
```

---

<small>Project organization strcuture inspired from the the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">Cookiecutter Data Science project template</a>. #cookiecutterdatascience</small>
