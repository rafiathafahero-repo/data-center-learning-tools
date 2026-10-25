# Automated Test Results — 25 October 2026 (WIB)

**Method:** Imported the saved three `.xlsx` workbooks into the workbook calculation engine; changed worksheet inputs; asserted recalculated results; exported/reopened; scanned formula error patterns. Tests were performed by ChatGPT in an automated execution environment, not by the user in Excel Desktop. All scenarios are synthetic.

**Final:** 37 PASS / 37 checks, 0 FAIL. Empty formula outputs may be represented as `""` or null; both are normalized as blank for this report.

## Availability — 12/12 PASS

| Scenario | Expected | Observed | Result |
|---|---|---|---|
| 2 units p=0 | 0 | 0 | PASS |
| 3 units p=0 | 0 | 0 | PASS |
| 2 units p=0.5 | 0.75 | 0.75 | PASS |
| 3 units p=0.5 | 0.875 | 0.875 | PASS |
| 2 units p=0.85 | 0.9775 | 0.9775 | PASS |
| 3 units p=0.85 | 0.996625 | 0.996625 | PASS |
| 2 units p=0.95 | 0.9974999999999999 | 0.9974999999999999 | PASS |
| 3 units p=0.95 | 0.999875 | 0.999875 | PASS |
| 2 units p=1 | 1 | 1 | PASS |
| 3 units p=1 | 1 | 1 | PASS |
| 8-layer serial system baseline | 0.5986697206181423 | 0.5986697206181423 | PASS |
| Expected annual downtime baseline | 3515.653247385074 | 3515.653247385074 | PASS |

## Readiness — 7/7 PASS

| Scenario | Expected | Observed | Result |
|---|---|---|---|
| Unassessed has no total score | blank | blank | PASS |
| Blank count assessed | 0 | 0 | PASS |
| Eligible excludes N/A | 29 | 29 | PASS |
| Assessed count | 3 | 3 | PASS |
| Coverage | 0.10344827586206896 | 0.10344827586206896 | PASS |
| Scoring among assessed | 0.5 | 0.5 | PASS |
| Reset clears score | blank | blank | PASS |

## Risk — 15/15 PASS

| Scenario | Expected | Observed | Result |
|---|---|---|---|
| Blank scenario shows unassessed | Not assessed | Not assessed | PASS |
| 1x5 score | 5 | 5 | PASS |
| 1x5 class | Low | Low | PASS |
| Summary count Low | 1 | 1 | PASS |
| 2x3 score | 6 | 6 | PASS |
| 2x3 class | Moderate | Moderate | PASS |
| Summary count Moderate | 1 | 1 | PASS |
| 3x5 score | 15 | 15 | PASS |
| 3x5 class | High | High | PASS |
| Summary count High | 1 | 1 | PASS |
| 4x5 score | 20 | 20 | PASS |
| 4x5 class | Very High | Very High | PASS |
| Summary count Very High | 1 | 1 | PASS |
| Missing impact prevents score | blank | blank | PASS |
| Reset clears count | 0 | 0 | PASS |

## Structural — 3/3 PASS

| Scenario | Expected | Observed | Result |
|---|---|---|---|
| Re-import 03_Data_Center_Risk_Register_Practice.xlsx | True | True | PASS |
| Re-import 01_Availability_Redundancy_Calculator.xlsx | True | True | PASS |
| Re-import 02_Data_Center_Readiness_Self_Assessment.xlsx | True | True | PASS |

## Verification limits

- No manual Excel Desktop or Google Sheets interactions were performed.
- These are sampled logical cases, not a proof of all input combinations.
- The automatic scan returned no `#REF!`, `#DIV/0!`, `#VALUE!`, `#NAME?`, or `#N/A` in examined saved workbooks.
- No real facility assessment, physical hardware inspection, independently measured uptime, or standard conformance audit took place.
- Spreadsheet data validation can be bypassed by imports/pastes in some software.
