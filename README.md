# Strategic Capital Allocation in Investment Banking
## A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024

**Author**: Ege Can  
**Academic Level**: Independent High-School Student Research (12th Grade)  
**Target Profile**: Warwick Business & Management BSc (2027 Entry)  
**Release Version**: `v1.0.0` (Publication Release)  
**Governing Standard**: Zero-Trust Empirical Research, Primary SEC EDGAR Filings, Non-Causal Observational Design  

---

## 1. Project Overview & Research Questions

How do leading financial institutions allocate capital between corporate reinvestment, balance-sheet capital retention, and shareholder distributions during periods of severe macroeconomic volatility? 

This study investigates the capital-allocation practices of eight prominent Wall Street investment-banking and financial advisory firms across the five-year period from 2020 through 2024.

### Core Research Questions:
1. **Primary Formulation**:
   > *"How do major investment-banking firms allocate capital between business investment, capital retention, and shareholder distributions, and how are these patterns associated with subsequent business performance?"*
2. **Refined Operational Formulation**:
   > *"To what extent are differences in capital retention and shareholder distribution associated with subsequent operating performance among major investment-banking firms?"*

### Epistemic Boundary:
This is an **observational, comparative, longitudinal study**. It documents empirical patterns and associations across two distinct business models. It does **not** assert causal mechanisms, prove optimal capital allocation strategies, or evaluate executive motives.

---

## 2. Sample Universe & Comparative Panel Architecture

To prevent false pooling across fundamentally different corporate balance sheets, the eight-firm universe is partitioned into two distinct analytical panels, with one firm evaluated as a standalone sensitivity context:

```
+----------------------------------------------------------------------------------------------------+
|                                    CANDIDATE UNIVERSE ARCHITECTURE                                 |
+------------------------------------+----------------------------------+----------------------------+
| PANEL A: Bank Holding Companies    | PANEL B: Independent Boutiques   | BROKER-DEALER SENSITIVITY  |
+------------------------------------+----------------------------------+----------------------------+
| - The Goldman Sachs Group (GS)     | - Evercore Inc. (EVR)            | - Jefferies Financial (JEF)|
| - Morgan Stanley (MS)              | - Lazard, Inc. (LAZ)             |   (Evaluated separately as |
| - JPMorgan Chase & Co. (JPM)       | - Moelis & Company (MC)          |   a non-bank broker-dealer |
| - Stifel Financial Corp. (SF)      |                                  |   sensitivity context)     |
+------------------------------------+----------------------------------+----------------------------+
```

### Rationale for Panel Separation:
- **Capital Definition**: For bank holding companies, "capital" represents regulatory solvency buffers (CET1, Tier 1 Leverage, SLR) mandated by the Federal Reserve to absorb credit and market shocks. For advisory boutiques, "capital" represents operational cash liquidity to fund payroll and partner draws through M&A advisory downturns.
- **Regulatory Framework**: Bank holding company payouts are governed by Federal Reserve Comprehensive Capital Analysis and Review (CCAR) stress tests. Advisory boutiques operate without statutory bank capital requirements.
- **Cost Structure**: Bank holding companies maintain substantial interest expense, credit loss provisions, and trading infrastructure. Advisory boutique costs are dominated by professional compensation expenses.

---

## 3. Key Empirical Findings

1. **Aggregate Shareholder Distributions**:
   Across the eight firms, an aggregate of **$233.2 billion** was returned to shareholders over 2020–2024, consisting of **$113.8 billion in cash dividends** and **$119.3 billion in common share repurchases**.
2. **Dividend Stability vs. Repurchase Fluctuation**:
   Cash dividends functioned as a stable or steadily increasing payout baseline across all firms (GS +92.5%, MS +124.1%, JPM +16.5%, SF +208.0%), whereas share repurchases exhibited wide cyclical variation that coincided with revenue expansions (peaking in 2021) and contractions.
3. **Regulatory Solvency Capital Ratios (Panel A)**:
   For Goldman Sachs, Morgan Stanley, and JPMorgan Chase, reported standardized Common Equity Tier 1 (CET1) ratios ranged from **13.1% to 17.4%** during 2020–2024. Stifel Financial reported a five-year average CET1 ratio of **11.24%** under its Category IV regional framework.
4. **Compensation Flexibility (Panel B)**:
   Advisory boutique compensation expense ratios rose from 60.1%–64.0% during the 2021 market boom to 66.0%–71.6% during the 2023 advisory trough, coinciding with operating margin compression from 20%–28% down to 5.1%–15.0% (and an operating loss at Lazard).
5. **Exploratory One-Year Lagged Associations ($t 	o t+1$)**:
   - **Panel A (Repurchases $	o$ Next-Year ROE)**: Near-zero linear association (Pearson $r = -0.049$, $p = 0.858$; Spearman $ho = -0.035$, $p = 0.897$, $N = 16$).
   - **Panel B (Repurchases $	o$ Next-Year Operating Margin)**: Negative linear association (Pearson $r = -0.403$, $p = 0.194$; Spearman $ho = -0.385$, $p = 0.217$, $N = 12$).
   - **Panel B (Advisory Fee Revenue $	o$ Next-Year Operating Income)**: Moderate positive association (Pearson $r = +0.470$, $p = 0.123$; Spearman $ho = +0.503$, $p = 0.095$, $N = 12$).

---

## 4. Central Author Interpretation

The primary conceptual interpretation developed by the author is:

> **"Financial outputs may reflect the interaction between financial conditions and the mechanisms through which firms make capital-allocation decisions."**

From this perspective:
- Identical financial accounting variables (such as "retained capital" or "share buybacks") carry distinct economic functions depending on a firm's business model, regulatory regime, and cost structure.
- Observed correlation patterns are non-causal associations shaped by the institutional and cyclical environments in which firms operate.

---

## 5. Summary of Limitations

1. **Small Exploratory Sample Sizes**: Lagged analysis is restricted to $N = 16$ (Panel A) and $N = 12$ (Panel B).
2. **Five-Year Window (2020–2024)**: Short longitudinal duration reflecting a unique macro cycle (pandemic relief, zero rates, 525 bps hiking cycle).
3. **Observational Design**: No causal inference or counterfactual testing.
4. **Unobserved Decision-Making**: Executive and boardroom deliberation processes are unobservable in 10-K filings.
5. **Within-Panel Heterogeneity**: Universal banks (JPM) differ from broker-dealer BHCs (GS, MS) and wealth networks (SF).
6. **One-Year Lag Horizon**: Multi-year strategic capital effects are not captured in single-year transitions.

---

## 6. Repository Structure & File Directory

```
project-banking/
├── README.md                              # Public release documentation & study overview
├── FINAL_PAPER.md                         # Complete publication-grade research manuscript (Markdown)
├── FINAL_PAPER.docx                       # Formatted Microsoft Word manuscript with tables & styles
├── FINAL_PAPER.pdf                        # 20-page camera-ready PDF with embedded high-res charts
├── FINAL_PAPER_SOURCE_MAP.csv             # Primary source audit map linking all 22 claims to SEC 10-K filings
├── FINAL_PAPER_QA.md                      # Quality assurance ledger confirming 20/20 criteria passed
├── PROJECT4_FINAL_FORENSIC_AUDIT.md       # Exhaustive forensic audit report across all project dimensions
│
├── PHASE3_RAW_DATA.csv                    # Audited primary dataset (540 cell-level observations)
├── PHASE3_DERIVED_DATA.csv                # Derived financial metrics (70 records with explicit formulas)
├── PHASE3_PROVENANCE_MAP.csv              # Exact cell-level SEC filing, table, and CIK provenance map
├── PHASE3_SOURCE_REGISTER.csv             # Register of all 40 primary SEC Form 10-K filings
├── PHASE3_QA_RESULTS.csv                  # Phase 3 data collection QA verification results
│
├── PHASE4_DESCRIPTIVE_STATISTICS.csv      # Five-year means, medians, standard deviations, min, max
├── PHASE4_FIRM_CHANGES.csv                # Absolute and percentage changes from 2020 to 2024
├── PHASE4_LAGGED_ASSOCIATIONS.csv         # One-year lagged transition pairs (t to t+1) for all panels
├── PHASE4_CORRELATIONS.csv                # Pearson r, Spearman rho, p-values, sample sizes
├── PHASE4_TABLES.md                       # Comprehensive empirical tables (Tables 1 through 8)
├── PHASE4_ANALYSIS_REPORT.md              # Descriptive and longitudinal analytical report
├── PHASE4_CHARTS/                         # High-resolution empirical visualizations (Charts 1 to 9)
│   ├── chart1_advisory_revenues.png
│   ├── chart2_distributions_timeline.png
│   ├── chart3_aggregate_distributions.png
│   ├── chart4_panel_a_cet1_ratios.png
│   ├── chart5_panel_a_roe.png
│   ├── chart6_panel_b_compensation_ratios.png
│   ├── chart7_panel_b_operating_margins.png
│   ├── chart8_scatter_repurchases_vs_roe.png
│   └── chart9_scatter_repurchases_vs_margins.png
│
├── PHASE5_DISCUSSION_DRAFT.md             # Author-led conceptual discussion draft
├── PHASE5_INTERPRETATION_MATRIX.csv       # Epistemic classification matrix (Observation vs Interpretation)
└── PHASE5_DISCUSSION_REPORT.md            # Final discussion synthesis report
```

---

## 7. Reproducibility & Verification Guide

### Primary Source Verification:
1. Open [`PHASE3_PROVENANCE_MAP.csv`](PHASE3_PROVENANCE_MAP.csv).
2. Every numerical value is mapped to a specific SEC Form 10-K filing, CIK code, fiscal year, Item number (Item 7 MD&A or Item 8 Financial Statements), and table title.
3. Access filings freely via the **SEC EDGAR database** (`https://www.sec.gov/edgar/searchedgar/companysearch`).

### Statistical Replication:
To replicate all correlations and descriptive statistics using Python standard library:
```bash
python3 -c "
import csv, math

with open('PHASE4_CORRELATIONS.csv') as f:
    for row in csv.DictReader(f):
        print(f"{row['panel']} | {row['predictor_variable']} -> {row['outcome_variable']}: r={row['pearson_r']}, rho={row['spearman_rho']}")
"
```

---

## 8. Release Metadata & Hash Verification

- **Release Tag**: `v1.0.0`
- **License**: Creative Commons Attribution 4.0 International (CC BY 4.0)
- **Author**: Ege Can (Independent Student Researcher)
