# DVW target species list

## Rationale

This repository contains the functionality to standardize the data of the target specie list as provided by [De Vlaamse Waterweg](https://www.vlaamsewaterweg.be/) (DVW) to a [Darwin Core Archive](https://www.gbif.org/darwin-core) that can be harvested by [GBIF](https://www.gbif.org/).

## Workflow

[source data](data/raw) → Darwin Core [mapping script](src/dwc_mapping.Rmd) → generated [Darwin Core files](data/processed)

## Published dataset

* [Dataset on the IPT](https://ipt.inbo.be/resource?r=dvw-target-list)
* [Dataset on GBIF](https://doi.org/10.15468/52b8h9)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md              : Description of this repository
├── LICENSE                : Repository license
├── dvw-target-list.Rproj  : RStudio project file
├── .gitignore             : Files and directories to be ignored by git
│
├── src
│   ├── dwc_mapping.Rmd    : Darwin Core mapping script
│   ├── _site.yml          : Settings to build website in docs/
│   └── index.Rmd          : Template for website homepage
│
├── docs                   : Repository website GENERATED
│
└── data
    ├── raw                : Source data, input for mapping script
    └── processed          : Darwin Core output of mapping script GENERATED
```

## Installation

<!-- This section is for users who want to download/adapt your checklist repository. You can leave it as is. -->

1. Click on `Use this template` to create a new repository on your account
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `docs/` (advanced)

## Contributors

[List of contributors](https://github.com/inbo/dvw-target-list/contributors)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
