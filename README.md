# Fertility and life expectancy in Bangladesh since 1950

How did Bangladesh's fertility and life expectancy change from 1950 on, and how does it compare with India, Pakistan and Nepal?

This is a small exploratory data analysis in R. It looks at the **total fertility rate** (average number of children per woman) and **life expectancy at birth** for four South Asian countries, 1950 to 2023.

## Key findings

<!-- Fill in AFTER you finish Phase 5/6, from your own computed numbers. 3 bullets max. Example shape:
- Fertility in Bangladesh peaked in <year> at <value> and fell to <value> by 2023.
- Compared with its neighbours: <one sentence>.
- Life expectancy and fertility: <one careful sentence, descriptive not causal>.
-->

_To be completed._

## Repository contents

| Path | What it is |
|---|---|
| `proj_1.Rmd` | The full analysis (R Markdown). Knit it to reproduce the report. |
| `Data/children-per-woman-un.csv` | Fertility data (see Data sources). |
| `Data/life-expectancy-hmd-unwpp.csv` | Life expectancy data (see Data sources). |
| `README.md` | This file. |

## How to run

1. Install R and RStudio.
2. Install the package: `install.packages("tidyverse")`.
3. Clone the repository and open `proj_1.Rmd` (open the project folder, so the relative paths `Data/...` work).
4. Click **Knit**, or run `rmarkdown::render("proj_1.Rmd")`.

## Data sources

Both files are downloaded from Our World in Data (OWID). Columns: `Entity`, `Code`, `Year`, and one value column.

| File | Measure | Underlying source | Years used |
|---|---|---|---|
| `children-per-woman-un.csv` | Total fertility rate | UN World Population Prospects, 2024 revision (via OWID) | 1950 to 2023 |
| `life-expectancy-hmd-unwpp.csv` | Life expectancy at birth, period | Human Mortality Database and UN WPP, combined (via OWID) | 1950 to 2023 used here; file goes back to 1751 for some countries |

Download pages (check these open the chart you expect, with no extra country selection in the URL):

- Fertility: https://ourworldindata.org/grapher/children-per-woman-un
- Life expectancy: https://ourworldindata.org/grapher/life-expectancy-hmd-unwpp

Date downloaded: <!-- fill in -->

Notes on the data:
- Values for recent years are UN **estimates** and are model-based, not direct counts. <!-- confirm which years are estimates vs projections in the 2024 edition -->
- Both files contain non-country rows (regions and aggregates, usually with a blank `Code`). The analysis keeps only `BGD`, `IND`, `PAK` and `NPL`.

## Licence and attribution

- **Data:** <!-- Check each provider's current terms before choosing: OWID's own licence statement on each chart page, the UN WPP terms, and the HMD user agreement. State here what you found, and if redistribution is not clearly allowed, delete the CSVs from the repo and rely on the download links above. -->
  Data are credited to: UN Population Division, *World Population Prospects 2024*; Human Mortality Database (University of California, Berkeley, and Max Planck Institute for Demographic Research); processed by Our World in Data.
- **Code:** released under the MIT Licence (add a `LICENSE` file, or replace this line with your choice).

## Limitations

- UN figures are modelled estimates built from censuses, surveys and registration data, so uncertainty is larger for earlier years and for countries with weaker records.
- This analysis is descriptive. Fertility and life expectancy moving in the same period does not show that one caused the other.
- Four countries only; results are not a statement about South Asia as a whole.

## References

- Lee, R. (2003). The demographic transition: three centuries of fundamental change. *Journal of Economic Perspectives*, 17(4), 167 to 190.
- <!-- Add the Bangladesh contraceptive use and fertility paper and any others you actually read, in a consistent format. -->

## Author

A. M. Mahin, Institute of Applied Statistics and Data Science, University of Dhaka.
