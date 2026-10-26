# Data Center Operations — Spreadsheet Learning Tools

Independent, **AI-assisted educational recreations** of three spreadsheet tools inspired by Data Center Management training materials. This public portfolio uses **synthetic data only**. The tool files were developed and programmatically tested with an assistant at the owner's request; it does **not** establish that the owner independently coded all the formulas or operated a production data center.

**Date:** 25 October 2026 (WIB) · **Scope:** Learning exercise, not an official ISO/IEC audit, Inixindo product, AWS tool, or measured facility assessment.

## Tools and screenshots

| Tool | Purpose | Preview | Main learning points |
|---|---|---|---|
| [Availability & Redundancy Calculator](workbooks/01_Availability_Redundancy_Calculator.xlsx) | Idealized parallel unit redundancy and serial service-chain availability | [Preview](evidence/01_Availability_Redundancy_Calculator_preview.png) | Input reliability, n-unit redundancy, annual expected downtime, independence assumptions |
| [Data Center Readiness Self-Assessment](workbooks/02_Data_Center_Readiness_Self_Assessment.xlsx) | 30 illustrative checks across 10 operating areas | [Preview](evidence/02_Data_Center_Readiness_Self_Assessment_preview.png) | Assessment coverage, evidence tracking, unknown ≠ failed, no ISO certification |
| [Risk Register Practice](workbooks/03_Data_Center_Risk_Register_Practice.xlsx) | Transparent 5 × 5 likelihood/impact model | [Preview](evidence/03_Data_Center_Risk_Register_Practice_preview.png) | Risk prioritization, explicit risk thresholds, scenario traceability |

## Start here

1. Review [Methodology and Assumptions](METHODOLOGY.md) to understand what each formula **can and cannot prove**.
2. Open any `.xlsx` in `workbooks/`. Work only with editable fields; use the **example inputs** rather than real private facility data.
3. Review [Test Results](TEST_RESULTS.md) and [machine-readable cases](test_cases.json). Automated evaluations were done using a spreadsheet calculation engine, not a real Microsoft Excel desktop session.
4. Use the [Evidence](evidence/) as worksheet renders, **not screenshots of a human operating Excel**.

## Results and boundaries

- **37 / 37 automated assertions passed** covering baseline, changed inputs, edge probabilities, readiness coverage/exclusion, risk classifications, missing values, and export/reopen checks.
- Three `.xlsx` workbooks inspected with **zero formula error matches** in programmatic scans. Saved calculator adds numeric validation to keep editable reliability input between `0` and `1`.
- The risk-register scale is an intentionally **custom learning convention**; it must not be represented as an ISO/IEC 22237 normative formula.
- Readiness scoring is **illustrative**, and unassessed rows do not silently count as failed controls. Coverage must be interpreted alongside assessed scores.
- Excel Desktop, Google Sheets, external standards compliance, reliability of real equipment, real AWS measurements, and onsite inspection have **not** been tested.
- The training originals remain private; their content is *not* included in this repository or reproduced verbatim.

## Source inspiration and licensing boundaries

The models were prompted by three privately provided course spreadsheets: *Calculating Availability*, *Data Center Audit – ISO 22237*, and *Analisa Resiko Berjenjang v1.1 – DC*. The third tool is **not a reproduction** of the original workbook's more elaborate scoring matrices. A fourth supplied file, *Metrik Pusat Data*, was treated as a reference only and is not part of this selected portfolio. The five private Inixindo PDFs are not redistributed. All substantive example data are hypothetical.

Official references for reading standard classification scope (not a statement of certification):
- [ISO/IEC 22237](https://www.iso.org/standard/78550.html)
- [Uptime Institute Tier classification](https://uptimeinstitute.com/tiers)

## LinkedIn & portfolio project description (honest attribution)

**Data Center Operations — Spreadsheet Learning Tools | Independent, AI-Assisted Learning Project**

Developed an educational portfolio with AI assistance to explore Data Center Operations concepts after completing instructor-led Data Center Management training. The portfolio contains three spreadsheet-based learning tools:

- **Availability & Redundancy Calculator:** Models idealized component redundancy, service-chain availability, and estimated downtime under explicitly stated assumptions.
- **Data Center Readiness Self-Assessment:** Uses 30 illustrative checks across 10 operational areas to practice assessment coverage and evidence tracking.
- **Risk Register Practice:** Applies a transparent 5 × 5 likelihood–impact model to fictional scenarios for risk identification and prioritization.

The repository includes documented assumptions, spreadsheet previews, example scenarios, and automated test results (**37/37 assertions passed**). The workbooks and programmatic tests were developed with an AI assistant at my request; this is an educational exercise using synthetic data, **not** independently coded production software, an official Inixindo assignment, an ISO/IEC compliance audit, or evidence of operating a live data center.

**Focus areas:** Data Center Fundamentals · Availability & Redundancy · Risk Assessment · Operational Readiness · Spreadsheet Modeling · Technical Documentation
