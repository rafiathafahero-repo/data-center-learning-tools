# Methodology and Assumptions

## 1. Availability & redundancy

The `Calculator` tab models the probability `p` that **one component is operational** at a randomly selected instant. Under *identical independent units* and ideal failover, availability with `n` parallel units is `A_parallel(n) = 1 - (1-p)^n`. Across eight independent serial stages, `A_system = PRODUCT(A_stage)`. Illustrative annual expected downtime is `(1-A_system) × 8760` hours. These are **assumptions**, not forecasts for a specific data center. No repair rates, correlated faults, maintenance windows, switching failures, regional disasters, or dependency architecture are represented.

Edited reliability inputs must lie in `0` to `1`; numeric data validation was added to `Calculator!B6:B13`. Pasted or imported values can bypass some spreadsheet validation, so check the inputs manually.

## 2. Readiness checklist

The `Checks` tab has **30 illustrative questions**, three each for 10 operating areas. Allowed statuses: `Implemented` (score `1`), `Partial` (`0.5`), `Not implemented` (`0`), `Not assessed` (excluded), `Not applicable` (excluded from eligible denominator). A blank record is not a failure. `Coverage = assessed count / eligible count`; `Assessed score = average scored status among assessed rows only`. The dashboard should show coverage and assessed score **together**; a 100% assessed score with only 10% coverage cannot be treated as 100% readiness. This checklist is **not ISO/IEC 22237 clause-by-clause assessment**, and no physical site is examined.

## 3. Risk register

The custom 5 × 5 learning model takes *likelihood* and *impact* as ordinal numbers from 1 to 5. `Risk score = likelihood × impact`. The purpose-built display thresholds are **Low (1–5)**, **Moderate (6–14)**, **High (15–19)**, and **Very High (20–25)**. This is a simple educational prioritization heuristic, not a regulatory or ISO normative risk formula. The editable register starts blank; synthetic examples live separately on `Examples & Tests`. Risk owners, assumptions, safeguards, and evidence should be recorded before using a rating for decision-making.

## Evidence and reproducibility

See `TEST_RESULTS.md` and `test_cases.json` for repeated test cases. Worksheet renders in `evidence/` are application-generated previews. They were **not** captured from Excel Desktop, nor from any production facility. All sensitive data are excluded and source training workbooks are not republished.
