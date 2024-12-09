# Building a Data Analysis pipeline tutorial

adapted from [Software Carpentry](http://software-carpentry.org/)

This example data analysis project analyzes the word count for all words in 4
novels. It reports the top 10 most occurring words in each book in a [report](doc/count_report.qmd).

## Current usage

### Set-up (first time only)

1. Clone this repo, and using the command line, navigate to the root of this project.

2. Run the following commands to create the conda environment:

    ```bash
    conda-lock install --name da-pipeline-make conda-lock.yml
    ```

3. Activate the conda environment:

    ```bash
    conda activate da-pipeline-make
    ```

### Run the analysis with GNU Make

Run the analysis:

```bash
make all
```

Reset the analysis the starting point:

```bash
make clean
```

### Run the analysis with Bash

Run the analysis:

```bash
bash runall.sh
```

## Depenedencies

- GNU Make
- Quarto
- Python & Python libraries:
  - `click`
  - `matplotlib`
  - `pandas`
