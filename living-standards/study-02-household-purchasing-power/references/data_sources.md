# Study 02 — Data Sources

## Research Period

2000–2024

---

# 1. Primary Source — Haut-Commissariat au Plan (HCP)

## 1.1 Consumer Price Index

Institution:

Haut-Commissariat au Plan (HCP)

Indicator:

Indice des prix à la consommation (IPC)

Purpose:

Measurement of consumer price dynamics and construction of the price-level component of the purchasing-power analysis.

Preferred coverage:

2000–2024

Official source:

HCP — Indice des prix à la consommation

Notes:

The exact CPI series, base year, frequency and methodology will be documented before integration into the final dataset.

---

# 2. Primary Source — HCP National Accounts

Institution:

Haut-Commissariat au Plan (HCP)

Indicator:

Household final consumption expenditure

Purpose:

Measurement of household consumption expenditure and contextualization of household economic conditions.

Preferred coverage:

2000–2024

Official source:

HCP — National Accounts

Notes:

The exact series and accounting definition will be verified before inclusion in the analytical dataset.

---

# 3. Complementary Source — World Bank

Institution:

World Bank

Database:

World Development Indicators

Country:

Morocco

Potential indicators:

- Households and NPISHs final consumption expenditure
- Households and NPISHs final consumption expenditure per capita
- Households and NPISHs final consumption expenditure, constant LCU
- Households and NPISHs final consumption expenditure, current LCU
- GDP per capita

Purpose:

Cross-checking, complementary analysis and internationally comparable indicators.

Important:

World Bank data will not automatically replace HCP data.

Where an HCP series is available and conceptually appropriate, HCP remains the preferred national source.

---

# 4. Bank Al-Maghrib

Institution:

Bank Al-Maghrib (BAM)

Potential indicators:

- household-related macroeconomic indicators;
- income-related indicators where available;
- monetary and price indicators;
- complementary national-account information.

Purpose:

Cross-validation and methodological comparison.

Important:

Only series with a clear definition and adequate temporal coverage will be considered.

---

# 5. IMF

Institution:

International Monetary Fund

Potential database:

World Economic Outlook

Purpose:

Complementary macroeconomic information where required.

Important:

IMF data will only be used when the variable definition is compatible with the research question and the primary national sources.

---

# 6. Source Selection Hierarchy

For identical or closely related indicators:

1. HCP
2. Bank Al-Maghrib
3. World Bank
4. IMF

This hierarchy is not absolute.

A lower-ranked source may be selected if it provides:

- better temporal coverage;
- a more appropriate definition;
- better methodological consistency;
- or a directly comparable series.

Any deviation from the hierarchy must be documented.

---

# 7. Data Selection Criteria

Every candidate series must satisfy the following criteria:

- official provenance;
- clearly documented definition;
- adequate temporal coverage;
- annual frequency;
- methodological consistency;
- reproducibility;
- compatibility with the research question.

---

# 8. Variables to Validate

The following variables will be investigated before construction of the final dataset:

## Mandatory

- year
- cpi
- household_consumption
- gdp_per_capita

## Candidate household-resource variables

- household_income
- disposable_income
- household_expenditure
- household_final_consumption

## Derived

- inflation
- real_income
- base100_income
- base100_cpi
- purchasing_power_index
- cumulative_inflation
- cumulative_income_growth
- income_gap
- pp_change

---

# 9. Critical Methodological Rule

No variable named `income_proxy` will be created until the underlying official series has been identified and its definition has been reviewed.

A macroeconomic variable such as GDP per capita must not be presented as household income.

Household purchasing power must be distinguished from:

- GDP per capita;
- household consumption;
- household expenditure;
- aggregate income;
- real wages.

---

# 10. CPI Harmonization

If CPI data are obtained from sources using different base years, the series must not be combined directly.

The selected CPI series will be transformed to a common analytical base only after verifying that the underlying index represents the same concept.

The preferred analytical reference for index comparisons is:

2010 = 100

provided that the transformation is methodologically valid.

---

# 11. Final Source Decision

The final dataset will be constructed only after:

1. identifying the exact official series;
2. downloading the original source data;
3. checking temporal coverage;
4. checking definitions;
5. checking units;
6. checking base years;
7. checking methodological breaks;
8. comparing overlapping sources where applicable.

The final source selection will be documented in the study methodology.

---

# 12. Reproducibility

The original downloaded files will be stored in:

data/raw/

Processed analytical datasets will be stored in:

data/processed/

No manually reconstructed source dataset will be treated as an original source.

---

# 13. Publication Rule

All figures, tables, notebooks and executive materials must ultimately derive from the validated processed dataset.

The processed dataset is the single analytical source of truth for Study 02.