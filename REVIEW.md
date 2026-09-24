# Workbook review

## Verified contents

Eight visible sheets; two Excel tables; three PivotTables; nine chart objects distributed across the workbook (including three dashboard charts). Data covers 142 countries, five continental groups and 12 observations per country at five-year intervals from 1952 to 2007. Each country-year has LIFE_EXP, POP_TOTAL and GDP_PC records.

There are 5,112 unique observation IDs, no duplicate country/year/indicator keys, and no stored Excel error values. The cleaned sheet adds 20,448 formula cells across four calculated columns. The supplied file was copied byte-for-byte and renamed to remove the doubled extension. No workbook contents were changed or recalculated in Excel during this review.

## Privacy and connections

No credential-like text was found in the shared strings. No external relationship targets, external workbook links, query tables, connection definitions, VBA parts, comments, hidden sheets, or explicitly hidden rows/columns were found. Core metadata includes the author's student display name. This is a bounded file inspection, not a guarantee that all possible sensitive content has been detected.

## Improvements to consider

1. Replace the UN-labelled internal report title with “Global Development Indicators — Analytical Insights Report”.
2. Link dashboard figures and insights to formula cells so they update with the data; correct “Expentency” to “Expectancy”.
3. Replace the static population number in calculated_fields!C8 with a verified SUMIFS formula if that skill is to be claimed.
4. Label chart averages as unweighted and state that Oceania includes two countries.
5. Add a precise source/version record and GDP-per-capita unit/base-year definition before drawing further economic comparisons.
6. Use per-indicator validation rules and distinguish missing values from zeros. Existing numeric/non-negative checks do not establish completeness or plausibility for every indicator.
7. Document how to expand fixed ranges and refresh PivotTables when adding observations.

The current saved dashboard chart caches contain the expected 12 years or five continents, excluding grand totals. Their PivotChart source ranges extend over totals, so generic spreadsheet renderers may not reproduce Excel's display exactly.

## Repository contents

Keep the workbook, README and this review. A checked dashboard image can be added as a preview. Exclude temporary Office files, duplicate workbook copies, personal assignment paperwork and operating-system files. A software requirements.txt would not describe this Excel project accurately.

## Preview compatibility

A preview was attempted with a non-Excel renderer. It did not preserve PivotTable filters and chart totals correctly, so that image is excluded from the package. Export the dashboard from Microsoft Excel for an accurate public screenshot. The original workbook was not re-exported or altered.
