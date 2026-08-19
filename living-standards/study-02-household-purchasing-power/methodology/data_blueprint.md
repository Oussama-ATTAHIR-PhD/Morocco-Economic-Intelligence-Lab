# Study 02 — Data Blueprint

## 1. Research Question

Has the purchasing power of Moroccan households improved or deteriorated between 2000 and 2024?

---

## 2. Analytical Objective

The objective is to measure the evolution of household purchasing power in Morocco by comparing the evolution of household economic resources with the evolution of consumer prices.

The analysis will distinguish clearly between:

- nominal values;
- real values;
- price dynamics;
- household consumption;
- purchasing power.

No indicator will be interpreted as a direct measure of household income unless the underlying source explicitly measures income.

---

## 3. Study Period

2007–2024

The study period is fixed and will not be changed unless data availability makes a specific variable impossible to construct consistently.

---

## 4. Primary Data Sources

### 4.1 Haut-Commissariat au Plan (HCP)

Priority source for:

- Consumer Price Index (CPI);
- household consumption;
- household income and expenditure indicators;
- household living-standard indicators;
- national accounts variables where applicable.

### 4.2 Bank Al-Maghrib (BAM)

Priority source for:

- macroeconomic indicators;
- household-related monetary indicators where available;
- complementary price and income information.

### 4.3 World Bank

Used as a complementary source for internationally comparable macroeconomic indicators when appropriate.

### 4.4 International Monetary Fund (IMF)

Used only where an appropriate official series is required and where the definition is compatible with the study methodology.

---

## 5. Core Variables

The final dataset will contain only variables that can be documented and justified.

### Required variables

- year
- cpi
- household_consumption
- gdp_per_capita

### Candidate variables

The following variables may be included only if a reliable and conceptually appropriate official series is identified:

- household_income
- household_final_consumption
- disposable_income
- household_expenditure
- inflation

---

## 6. Variable Definitions

### year

Calendar year.

### cpi

Consumer Price Index.

The exact CPI definition, base year, geographic coverage and source will be documented before analysis.

### household_consumption

Household consumption expenditure measured according to the definition provided by the official source.

### gdp_per_capita

GDP per capita used only as a macroeconomic contextual indicator and never treated as a direct household-income measure.

### household_income

Household income will only be used if an official series with adequate temporal coverage and methodological consistency is identified.

### inflation

Annual inflation rate derived from the CPI series or taken directly from an official source, provided that the definition is documented.

---

## 7. Harmonization Rules

All annual variables must use the same calendar-year frequency.

All monetary variables must be documented in:

- currency;
- nominal or real terms;
- current or constant prices;
- base year where applicable.

Price indices must not be combined across incompatible base years without an explicit rebasing or index transformation.

When a series is rebased, the transformation must preserve its relative annual movements.

No value will be manually altered to force consistency between sources.

---

## 8. Purchasing Power Measurement

The primary purchasing-power concept will be based on the relationship between an economic resource indicator and the price level.

The preferred formulation is:

Purchasing Power Index = Real Economic Resource Index

where the nominal economic resource indicator is deflated using the CPI.

The exact indicator used will depend on the availability and methodological quality of the official income/resource series.

If no sufficiently consistent household-income series is available for the full 2000–2024 period, the study will not fabricate a household-income measure.

Instead, the analysis will explicitly use a documented proxy and clearly label it as such.

---

## 9. Base Year

For comparative index analysis, 2010 = 100 will be used where compatible with the underlying data.

If the official source uses another base year, the series will be rebased mathematically rather than mixing incompatible index bases.

---

## 10. Derived Variables

Subject to data availability, the following variables will be constructed:

- inflation
- real_income
- base100_income
- base100_cpi
- purchasing_power_index
- cumulative_inflation
- cumulative_income_growth
- income_gap
- pp_change

Every derived variable must have a documented mathematical definition.

---

## 11. Data Quality Requirements

Before analysis:

- check missing values;
- check duplicate years;
- check numerical types;
- check extreme values;
- check breaks in series;
- check methodological changes;
- check changes in CPI base;
- check changes in variable definitions;
- compare overlapping series where multiple official sources exist.

---

## 12. Source Hierarchy

When several sources provide the same indicator, the following hierarchy applies:

1. HCP
2. Bank Al-Maghrib
3. World Bank
4. IMF

The hierarchy may be overridden only when the lower-ranked source provides a demonstrably more appropriate series for the exact research variable.

Any such decision must be documented.

---

## 13. Data Integrity Principle

The study will prioritize methodological consistency over completeness.

A shorter but conceptually consistent series is preferable to a longer series combining incompatible definitions.

No data point will be invented, estimated or manually modified without explicit methodological justification.

---

## 14. Final Dataset Principle

The final processed dataset must be:

- machine-readable;
- documented;
- reproducible;
- traceable to official sources;
- free of manually entered analytical results.

The processed dataset will be the single source of truth for all notebooks and visualizations.

---

## 15. Reproducibility Principle

All calculations must be performed programmatically.

Charts must be generated directly from the processed dataset.

Values displayed in reports and LinkedIn materials must originate from the analytical outputs.

No numerical value will be manually recreated in presentation material.

---

## 16. Publication Principle

Before publication, the following must be identical across:

- processed CSV;
- notebooks;
- figures;
- tables;
- executive summary;
- GitHub README;
- LinkedIn carousel.

Any discrepancy must be corrected before publication.

---

## 17. Research Integrity

The study will distinguish between:

- measured household purchasing power;
- macroeconomic proxies;
- descriptive associations;
- causal relationships.

No causal conclusion will be made unless supported by an appropriate identification strategy.

The study will explicitly state its limitations.

---

## 18. Final Decision Rule

The final purchasing-power indicator will be selected only after reviewing the available official data.

The selection will be based on:

1. conceptual relevance;
2. official provenance;
3. temporal coverage;
4. methodological consistency;
5. reproducibility;
6. interpretability.

Once selected and documented, the indicator definition becomes fixed for the study.