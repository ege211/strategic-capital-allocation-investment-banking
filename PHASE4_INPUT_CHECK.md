# Phase 4 Input Check: Pre-Analysis Data Audit

**Project Title**: Strategic Capital Allocation in Investment Banking (2020–2024)  
**Author**: 12th-Grade Independent Student Research Project  
**Date**: September 2026  
**Status**: Pre-Analysis Verification Complete — All Datasets Reconciled

---

## 1. Overview of Pre-Analysis Input Audit

Before calculating any descriptive statistics, within-firm changes, or lagged associations in Phase 4, I performed a complete automated consistency check across all Phase 3 data artifacts:
- `PHASE3_RAW_DATA.csv` (Primary audited observations)
- `PHASE3_DERIVED_DATA.csv` (Explicitly calculated metrics)
- `PHASE3_PROVENANCE_MAP.csv` (Filing citations, accession numbers, and URLs)
- `PHASE3_SOURCE_REGISTER.csv` (Registered Form 10-K primary filings)
- `PHASE2_DATA_DICTIONARY.csv` (Locked variable taxonomy and accounting bases)

The purpose of this check is to guarantee that the analysis is built on a 100% verified, consistent foundation with zero fabricated observations, no temporal leaks, and complete provenance tracking.

---

## 2. Dataset Dimensions and Summary Counts

| Dimension | Checked Item | Expected Value | Verified Value | Reconciliation Status |
| :--- | :--- | :---: | :---: | :---: |
| **Total Firms** | Unique candidate & sensitivity tickers | 8 firms | 8 firms | **MATCH** |
| **Fiscal Years** | Annual periods covered | 5 years (2020–2024) | 5 years | **MATCH** |
| **Temporal Bounds** | Observations from 2025 or 2026 | 0 | 0 | **MATCH** |
| **Primary Filings** | Audited SEC Form 10-K annual reports | 40 filings | 40 filings | **MATCH** |
| **Raw Data Rows** | Primary reported observations | 540 rows | 540 rows | **MATCH** |
| **Raw Variables** | Unique variables in raw data | 19 variables | 19 variables | **MATCH** |
| **Derived Rows** | Calculated observations | 70 rows | 70 rows | **MATCH** |
| **Derived Variables**| Unique derived metrics | 3 variables | 3 variables | **MATCH** |
| **Provenance Records**| Traceable filing citations | 540 records | 540 records | **MATCH** |
| **ID Alignment** | Raw IDs matching Provenance IDs | 100% (540/540) | 100% (540/540) | **MATCH** |
| **Derived Lineage** | Input IDs present in raw data | 100% (70/70) | 100% (70/70) | **MATCH** |

---

## 3. Coverage by Firm and Panel Grouping

The audit confirmed the exact panel architecture established in Phase 1 and maintained through Phase 3:

### Main Panel A: Bank Holding Companies (4 Firms)
- **Goldman Sachs (`GS`)**: 5 fiscal years (2020–2024), FY ends Dec 31.
- **Morgan Stanley (`MS`)**: 5 fiscal years (2020–2024), FY ends Dec 31.
- **JPMorgan Chase (`JPM`)**: 5 fiscal years (2020–2024), FY ends Dec 31.
- **Stifel Financial (`SF`)**: 5 fiscal years (2020–2024), FY ends Dec 31.

### Main Panel B: Independent Advisory Boutiques (3 Firms)
- **Evercore (`EVR`)**: 5 fiscal years (2020–2024), FY ends Dec 31.
- **Lazard (`LAZ`)**: 5 fiscal years (2020–2024), FY ends Dec 31.
- **Moelis & Company (`MC`)**: 5 fiscal years (2020–2024), FY ends Dec 31.

### Sensitivity / Context Group (1 Firm)
- **Jefferies Financial Group (`JEF`)**: 5 fiscal years (2020–2024), FY ends Nov 30.
- *Isolation Status*: Jefferies is strictly quarantined from Panel A and Panel B pooling due to its non-bank regulatory charter (SEC Rule 15c3-1) and non-calendar fiscal year-end.

---

## 4. Status Label and Accounting Consistency Audit

Every observation in `PHASE3_RAW_DATA.csv` has an explicit status label. There are zero unexplained blank or empty numerical cells:

1. **`DIRECT` (450 observations)**:
   - Numerical values extracted verbatim from official 10-K financial statements or disclosure tables.
2. **`DERIVED` in Raw Table (15 observations)**:
   - Operating margin for advisory boutiques (`EVR`, `LAZ`, `MC` across 5 years), computed from reported operating income and net revenue.
3. **`UNAVAILABLE` (5 observations)**:
   - Moelis & Company (`MC`) operating communications/technology expense across 2020–2024. Moelis does not disclose a separate line item for technology in its 10-K filings. These values are explicitly marked `UNAVAILABLE` and are never converted to zero.
4. **`NOT_APPLICABLE` (20 observations)**:
   - Stifel (`SF`) Supplementary Leverage Ratio (5 years): Stifel is a Category IV regional bank and is legally exempt from calculating or publishing SLR under Federal Reserve rules.
   - Jefferies (`JEF`) Basel III capital measures (`cet1_standardized`, `tier1_leverage_ratio`, `supplementary_leverage_ratio` across 5 years = 15 observations): Jefferies is regulated under broker-dealer net capital rules rather than Federal Reserve bank holding company rules.
   - All 20 cells are explicitly labelled `NOT_APPLICABLE` and are never converted to zero.
5. **`STRUCTURALLY_NON_COMPARABLE` (50 observations)**:
   - Balance-sheet cash and long-term wholesale debt for non-boutiques (`GS`, `MS`, `JPM`, `SF`, `JEF` across 5 years = 50 observations). Bank cash represents central bank reserve balances and clearing deposits, while bank debt funds trading assets and loan portfolios. In contrast, boutique cash represents corporate liquid cushions and debt represents corporate senior notes. These are preserved for individual context but quarantined from pooled cross-business models.

---

## 5. Temporal Integrity and Fiscal Year Alignment

- **2025 / 2026 Exclusion**: Verified that exactly 0 observations belong to fiscal years 2025 or 2026.
- **Fiscal Year-End Integrity**:
  - All seven firms in Panel A and Panel B end their fiscal year on **December 31**.
  - Jefferies Financial Group (`JEF`) ends its fiscal year on **November 30** (e.g., FY 2020 period ended 2020-11-30). This difference is preserved throughout all data tables.

---

## 6. Audit Conclusion & Phase 4 Clearance

The pre-analysis consistency audit identified **zero data inconsistencies, zero missing values without explicit labels, and zero temporal leaks**.

- Raw data rows: 540 (100% reconciled to provenance map)
- Derived data rows: 70 (100% traced to valid raw inputs)
- Quality status: **PASSED AND VERIFIED**

The dataset is verified and cleared for Phase 4 descriptive statistics, within-firm longitudinal analysis, and exploratory lagged comparisons.
