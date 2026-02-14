Clean Data Mini Project
Dataset Cleaning Steps & Rationales

1. Age

Type: numeric

Missing values: filled with median

Outliers: capped at 1st and 99th percentile

Rationale: Median is robust to outliers; capping reduces the effect of extreme values

2. Income

Type: numeric

Missing values: filled with median

Outliers: capped at 99th percentile

Rationale: Median is robust; capping high salaries reduces noise

3. City

Type: categorical

Missing values: filled with 'unknown'

Cleaning: strip spaces and convert to lowercase

Rationale: standardizes text for analysis and mapping

4. Signup Time

Type: datetime

Missing/invalid: converted to NaT

Timezone: UTC

Rationale: unify time for temporal analysis

Flags

age_missing and income_missing indicate where missing values were imputed

Limitations / Trade-offs

Capping may remove valid extreme values

Median imputation may slightly skew distribution if missing values are high
