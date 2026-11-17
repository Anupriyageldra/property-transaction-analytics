# Property Transaction Analytics & Market Insights

An R-based data analytics project that transforms real estate transaction data into meaningful market insights through statistical analysis, data visualization, neighbourhood-level analysis, and automated narrative reporting.

The project generates a comprehensive HTML report containing **10 different analytical narratives**, each presenting the property transaction data from a distinct perspective. It aims to make real estate data easier to understand, interpret, and use for informed decision-making.

---

## Project Overview

Real estate transaction datasets contain valuable information about property prices, transaction values, property sizes, geographical locations, and market activity. However, extracting meaningful insights from raw transaction records requires systematic data processing, statistical analysis, and effective visualization.

This project uses **R programming** to automate the analysis of property transaction data and generate a single, interactive-style HTML report with multiple narrative formats.

The analysis focuses on identifying transaction patterns, understanding property price trends, comparing neighbourhood performance, examining transaction distributions, and highlighting data quality issues.

## Key Features

- **Automated Data Processing:** Imports and prepares Excel-based property transaction datasets for analysis.
- **Transaction Trend Analysis:** Examines transaction activity and changes over time.
- **Property Price Analysis:** Evaluates transaction values, property areas, and price per square metre.
- **Neighbourhood Analysis:** Compares transaction activity and property market performance across neighbourhoods.
- **Geographical Insights:** Analyses transaction distribution across available zones and neighbourhoods.
- **Statistical Analysis:** Calculates descriptive statistics, including mean, median, minimum, maximum, and distribution measures.
- **Data Quality Assessment:** Identifies missing values, inconsistencies, and potential outliers.
- **Data Visualization:** Generates charts and graphical summaries to communicate analytical findings.
- **Automated Report Generation:** Produces one consolidated HTML report containing 10 different analytical writing styles.

## Ten Analytical Report Styles

The project presents the same underlying dataset through ten distinct reporting perspectives:

| No. | Report Style | Focus |
|---|---|---|
| 1 | Formal Analytical Report | Structured analysis of transaction data and market indicators |
| 2 | Executive Briefing | Concise findings and key business insights |
| 3 | Technical & Statistical Report | Statistical measures, distributions, and analytical observations |
| 4 | Descriptive Market Narrative | Overall property market behaviour and transaction patterns |
| 5 | Data Quality & Governance Report | Missing values, inconsistencies, and data reliability |
| 6 | Geographic & Neighbourhood Analysis | Comparison of zones and neighbourhood-level activity |
| 7 | Investor-Oriented Report | Property pricing patterns and potential investment insights |
| 8 | Policy & Urban Planning Report | Market observations relevant to planning and development |
| 9 | Plain-Language Report | Easy-to-understand explanations of analytical findings |
| 10 | Research & Recommendations Report | Consolidated observations and data-driven recommendations |

## Technology Stack

The project is developed using R and its data analysis and visualization ecosystem.

| Technology | Purpose |
|---|---|
| R | Core programming and statistical analysis |
| RStudio | Development environment |
| openxlsx | Reading Excel datasets |
| dplyr | Data manipulation and transformation |
| tidyr | Data cleaning and restructuring |
| lubridate | Date processing and time-based analysis |
| ggplot2 | Data visualization |
| scales | Formatting numerical values and chart labels |
| glue | Dynamic report text generation |
| stringr | Text processing |
| htmltools | HTML report generation |
| knitr | Report formatting |

## Project Structure

```text
property-transaction-analytics/
│
├── R/
│   └── generate_reports.R
│
├── data/
│   └── README.md
│
├── output/
│   └── .gitkeep
│
├── .gitignore
├── LICENSE
└── README.md
```

### Directory Description

- **R/** – Contains the main R script responsible for data processing, analysis, visualization, and report generation.
- **data/** – Directory for storing the input Excel dataset. The original dataset is not included in the repository.
- **output/** – Stores the generated HTML report and supporting visualization assets.
- **generate_reports.R** – Main execution script.
- **.gitignore** – Excludes unnecessary files and generated content from version control.
- **LICENSE** – Defines the project's licensing terms.

## Dataset Description

The project is designed to work with an Excel-based property transaction dataset.

The expected dataset includes fields such as:

| Column | Description |
|---|---|
| TRANSACTION.DATE | Date of the property transaction |
| VALUE..SAR. | Total transaction value in Saudi Riyals |
| TRANSACTION.AREA..sqm. | Area of the transacted property in square metres |
| PROPERTY.TRANSACTION.RATE..SAR.sqm. | Transaction rate per square metre |
| ZONE | Geographical zone |
| NEIGHBORHOOD | Neighbourhood associated with the property |
| PROPERTY.UID | Unique property identifier |
| PROPERTY.TYPE.ESTATER | Property type according to the available estate records |
| PROPERTY.TYPE.AS.PER.GOVERNMENT.RECORD | Property type according to government records |
| OUTLIER | Outlier indicator, where available |

**Note:** The dataset is not included in this repository. Users must provide their own dataset with compatible column names and data structure. Some analyses may require optional columns.

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Anupriyageldera/property-transaction-analytics.git
```

### 2. Open the Project

Open the downloaded repository folder in RStudio.

### 3. Install Required Packages

Run the following command in the R console:

```r
packages <- c(
  "openxlsx",
  "dplyr",
  "lubridate",
  "ggplot2",
  "scales",
  "glue",
  "tidyr",
  "stringr",
  "htmltools",
  "knitr"
)

install.packages(packages)
```

### 4. Add Your Dataset

Place your Excel dataset inside the `data/` directory.

The expected filename is:

```text
property_transactions_1750066258149.xlsx
```

If the dataset is stored elsewhere or has a different filename, the script can prompt you to select it.

### 5. Execute the Analysis

Run the main R script:

```r
source("R/generate_reports.R")
```

The script processes the dataset, performs the configured analyses, generates visualizations, and creates the consolidated HTML report.

## Output

After successful execution, the generated report will be available at:

```text
output/property_transaction_10_reports.html
```

Supporting visualization assets will be stored in:

```text
output/report_assets/
```

The HTML report brings together the ten analytical narratives in one place, making it easier to review the findings from business, statistical, geographical, and research perspectives.

## Analytical Objectives

The primary objectives of this project are:

1. Understand property transaction patterns and market activity.
2. Examine property transaction values and price-per-square-metre trends.
3. Identify neighbourhoods with different levels of transaction activity.
4. Compare geographical distribution across available zones.
5. Evaluate the quality and consistency of the underlying dataset.
6. Communicate analytical findings through meaningful visualizations.
7. Automate the creation of multiple report formats using R.

## Applications

This project demonstrates how data analytics can support:

- Real estate market research.
- Property transaction monitoring.
- Neighbourhood-level market comparisons.
- Investment research and property valuation analysis.
- Urban development and planning studies.
- Business intelligence and analytical reporting.

## Future Enhancements

Potential improvements include:

- Interactive dashboards using Shiny or Power BI.
- Predictive property price modelling using machine learning.
- Advanced geographical visualization using GIS.
- Automated anomaly detection for unusual transactions.
- Integration with regularly updated property transaction datasets.
- Exporting analytical reports to PDF and Excel formats.

## Limitations

- The quality of the analysis depends on the completeness and accuracy of the input dataset.
- Findings represent patterns in the supplied transaction records and should not automatically be interpreted as predictions of future property prices.
- Geographical conclusions are limited to the location fields available in the dataset.
- The generated report requires a compatible input Excel file.

## Author

**Anupriya Geldra**

