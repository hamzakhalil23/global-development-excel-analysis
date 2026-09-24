# Global Development Analysis in Excel

An Excel portfolio project exploring life expectancy, population and GDP per capita across 142 countries in five continental groups, using 5,112 indicator observations from 1952–2007.

## Open the project

Download [global-development-analysis.xlsx](global-development-analysis.xlsx) and open it in Microsoft Excel. Start with **dashboard**, then explore **Insights_Report**, **pivot_analysis** and the supporting sheets. The workbook contains its data; no credentials or separate dataset download are required. Excel is recommended for the original PivotTables and chart layout. No Python requirements file is needed.

## Workbook contents

| Sheet | Purpose |
| --- | --- |
| raw_data | 5,112 observations: 142 countries × 12 sampled years × 3 indicators |
| cleaned_data | Original data plus value checks, decade grouping, life-expectancy bands and indicator lookups |
| quality_checks | Counts, missing-ID checks, year/value bounds and review flags |
| calculated_fields | Formula explanations, indicator mapping and summary metrics |
| pivot_analysis | Three PivotTables comparing indicators by continent and year |
| charts | Supporting charts |
| dashboard | Three charts, headline figures and narrative findings |
| Insights_Report | Written interpretation of the analysis |

## Excel techniques demonstrated

- Excel tables and three PivotTables, with charts for trends and continental comparisons.
- `IF`, `AND`, `ISNUMBER`, `FLOOR` and `VLOOKUP` for calculated columns.
- `COUNTA`, `COUNTBLANK`, `COUNTIF`, `AVERAGEIF`, `MIN` and `MAX` for checks and summaries.
- `INDEX`, `MATCH` and `TEXT` for formatted analytical results.

## Selected results

- Mean life expectancy across all sampled country-year records: **59.47 years**.
- Change in mean life expectancy from 1952 to 2007: **+15.67 years in Africa** and **+24.41 years in Asia**.
- Oceania has the highest 2007 mean life expectancy (**80.72 years**) and mean GDP per capita (**29,810.19**, in the source-defined units) among the represented continental groups.
- The represented Asian countries have a combined 2007 population of approximately **3.81 billion**.

These figures were independently checked against the embedded raw observations during preparation for GitHub.

## Data source and interpretation

The workbook's source note identifies a **Gapminder/Plotly country-year extract reshaped to long indicator format for education**. Its original filename and report title contain “UN”, but the workbook does not establish UN authorship, employment or affiliation. SDG labels are educational mappings.

Source references: [Plotly's Gapminder CSV](https://github.com/plotly/datasets/blob/master/gapminderDataFiveYear.csv), [Gapminder data and attribution guidance](https://www.gapminder.org/data/), and [Gapminder reuse terms](https://www.gapminder.org/free-material/). The exact historical download/version was not recorded in the workbook, so the Plotly link is a reference rather than a verified byte-for-byte source.

Based on free material from GAPMINDER.ORG, CC-BY LICENSE. Underlying data rights remain with their respective sources; this repository does not replace those terms.

## Limitations

- This is descriptive analysis of a historical sample, not a current or complete global dataset. Oceania contains only Australia and New Zealand.
- Life-expectancy and GDP-per-capita means are unweighted country averages. The overall life-expectancy figure also averages across sampled years; it is not a current population-weighted global statistic.
- Raw and cleaned sheets retain identical values in the original 12 columns. The workbook demonstrates validation and enrichment, but does not document corrections to dirty records.
- Dashboard headline figures and narrative text are static. Refresh PivotTables and manually check these labels after changing data. Some formulas use fixed row ranges.
- `calculated_fields!C8` is labelled SUMIFS but stores a fixed value. SUMIFS implementation is not claimed.
- The quality-check minimum and maximum combine indicators with different units; they are bounds checks, not comparable development metrics.
- The original workbook is preserved unchanged, including its original internal report title and minor spelling errors.

See [REVIEW.md](REVIEW.md) for the inspection details and suggested improvements.
