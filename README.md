# Climate and Environmental Justice Tools and Publications

This repository hosts the **analysis**, **datasets**, and **supporting materials** for a data story on climate and environmental justice tools and research publications.It brings together citation data, metrics, and visualizations to explore how these tools are developed, applied, and studied.

## Repository Structure

```text
climate-ej-tools-publications/
│
├── 01_raw_data/           # Original datasets downloaded from external sources — never modified
├── 02_processed_data/     # Cleaned and manually coded datasets — finalized versions ready for analysis
├── 03_codebooks/          # Documentation defining coding categories (for studies, publishers, etc.)
├── 04_metrics_data/       # Google Scholar or bibliometric metrics collected at data extraction time
├── 05_cleaned_datasets/   # RDS files with cleaned, merged, and stratified samples ready for visualization or modeling
├── 06_viz_ready/          # Data prepared specifically for visualization dashboards, plots, or reports
│
├── scripts/               # R scripts or helper functions for automation
├── docs/                  # Documentation, notes, and supporting materials
└── README.md
```

## Getting Started

### 1️⃣ Clone this repository

```bash
git clone https://github.com/<your-username>/climate-ej-tools-publications.git
cd climate-ej-tools-publications
```

### 2️⃣ Install required R libraries

Before running the analysis, install and load the following R libraries:

```R
# Folder structure helpers
library(here)
library(readr)
library(ezknitr)

# Data cleaning & analysis
library(tidyverse)
library(janitor)
library(lubridate)
library(stringr)
library(forcats)
library(vcd)

# Visualization
library(highcharter)
library(igraph)
library(RColorBrewer)
library(htmlwidgets)
library(gt)
```

To install them all at once:

```R
install.packages(c(
  "here", "readr", "ezknitr",
  "tidyverse", "janitor", "lubridate", "stringr", "forcats", "vcd",
  "highcharter", "igraph", "RColorBrewer", "htmlwidgets", "gt"
))
```

### 3️⃣ Reproduce or Extend the Analysis

To reproduce or extend the analysis, see the main Quarto script:

```bash
analysis.qmd
```

Render the main report using Quarto:

```bash
quarto render analysis.qmd
```

This will generate all tables, charts, and relevant output.

## References and Licensing

- `references.bib` — Bibliography file

- `LICENSE` — License for repository use
