# Before You Run the Test

**A decision-based guide to statistical analysis in aquatic sciences for young scientists**

This repository contains the reproducible R tutorial that accompanies the article
*How to Choose Your Statistical Test Before You Run It*, submitted to
**Limnology and Oceanography Bulletin**.

The tutorial walks through the complete cycle of an environmental data analysis,
using a deliberately messy simulated dataset from a fictitious coastal system,
the Aura Estuary:

1. Building a research question with a defined anatomy
2. Stating an *a priori* hypothesis, and distinguishing confirmatory from exploratory posture
3. Diagnosing a messy dataset (sensor errors, mixed data types, inconsistent categories, duplicates)
4. Cleaning it with the `tidyverse`
5. Choosing a statistical test from the study design rather than from the results
6. Running the test and reporting the finding with its limits attached

The guiding idea is simple: **you choose your test from the structure of your
data and your design, never from the answer it gives you.**

## Reading the tutorial

The rendered tutorial displays directly on GitHub:

**[before-you-run-the-test.md](before-you-run-the-test.md)**

No installation is needed to read it. Everything below is only for readers who
want to run the code themselves.

## Running the code

You will need [R](https://cran.r-project.org/) and
[Quarto](https://quarto.org/docs/get-started/). Install the packages used here:

```r
install.packages(c("dplyr", "tidyr", "ggplot2", "plotly", "stringr", "lubridate"))
```

Then render:

```bash
quarto render before-you-run-the-test.qmd
```

The dataset is generated inside the tutorial with a fixed random seed, so no
external data file is required and the results are identical on every machine.

## Repository contents

| File | What it is |
|---|---|
| `before-you-run-the-test.qmd` | Source of the tutorial (Quarto + R) |
| `before-you-run-the-test.md` | Rendered version, displayed by GitHub |
| `before-you-run-the-test_files/` | Figures produced during rendering |
| `CITATION.cff` | Citation metadata |
| `LICENSE` | MIT license (code) |

## Citation

Citation details and a permanent DOI will be added here once the accompanying
article is published. In the meantime, please cite this repository using the
metadata in `CITATION.cff`.

## License

Code is released under the [MIT License](LICENSE). The tutorial text and figures
are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## Authors

Juline Rodrigues da Conceição and Stéfano Zorzal-Almeida
