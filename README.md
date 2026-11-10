# Strategic Capital Allocation in Investment Banking
### A Comparative Longitudinal Study of Major U.S. Firms (2020 to 2024)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Academic Level](https://img.shields.io/badge/Level-High%20School%20Student%20Research-blue.svg)](#)
[![Data Source](https://img.shields.io/badge/Data-SEC%20Form%2010--K%20Filings-green.svg)](https://www.sec.gov/edgar)

> **An independent high-school student research project analyzing how leading Wall Street investment banks and advisory boutiques allocated capital between balance-sheet retention, reinvestment, and shareholder distributions during periods of macroeconomic volatility.**

---

## 1. Student Researcher's Note & Motivation

**Author:** Ege Umut Can  
**School:** FMV Işık High School, Istanbul (Class of 2027)  
**Research Focus:** Corporate Finance, Capital Structure & Banking Regulation  

### Why I Undertook This Study:
When studying introductory economics and corporate finance, capital allocation is often taught through simple textbook formulas. Yet in the real financial world, executive leadership faces difficult trade-offs: *Should excess cash be returned to shareholders via buybacks and dividends, held on the balance sheet as a regulatory cushion, or reinvested into employee compensation and technology?*

Between 2020 and 2024, the global economy witnessed a rapid sequence of shocks: the initial COVID-19 pandemic shutdown and emergency stimulus (2020), an explosive boom in corporate mergers and IPOs (2021), followed by the steepest Federal Reserve interest-rate hiking cycle in four decades (2022 to 2023), and subsequent market stabilization (2024).

To understand how real-world financial institutions reacted to these rapid shifts, I hand-collected and analyzed financial data from **40 official SEC Form 10-K annual reports** across eight prominent Wall Street institutions.

---

## 2. Research Scope & Candidate Universe

### Core Research Question:
> *"How do major investment-banking firms allocate capital between business investment, capital retention, and shareholder distributions, and how are these patterns associated with subsequent business performance?"*

### Two Distinct Business Models (Analytical Panels):
To avoid comparing fundamentally incomparable institutions, the eight firms were grouped into two distinct analytical panels:

```text
┌───────────────────────────────────────┐       ┌───────────────────────────────────────┐
│     PANEL A: Bank Holding Companies   │       │     PANEL B: Independent Boutiques    │
├───────────────────────────────────────┤       ├───────────────────────────────────────┤
│ • The Goldman Sachs Group (GS)        │       │ • Evercore Inc. (EVR)                 │
│ • Morgan Stanley (MS)                 │       │ • Lazard, Inc. (LAZ)                  │
│ • JPMorgan Chase & Co. (JPM)          │       │ • Moelis & Company (MC)               │
│ • Stifel Financial Corp. (SF)         │       │                                       │
│                                       │       │ Standalone Context:                   │
│ Focus: Balance-sheet intensive,       │       │ • Jefferies Financial Group (JEF)     │
│ subject to Federal Reserve stress     │       │                                       │
│ tests and strict CET1 solvency rules. │       │ Focus: Asset-light advisory models,   │
└───────────────────────────────────────┘       │ compensation-driven, high cash payout.│
                                                └───────────────────────────────────────┘
```

---

## 3. Key Findings & Takeaways

1. **$233.3 Billion in Shareholder Distributions:**
   Across the eight firms over the 2020–2024 period, a combined **$233.3 billion** was returned to equity holders ($113.9 billion in regular cash dividends and $119.4 billion in share repurchases).
2. **Dividends as a Stable Anchor vs. Cyclical Buybacks:**
   Bank dividends rose over the period and worked as a baseline payout (Lazard and Moelis cut theirs). Common share repurchases fluctuated widely: they jumped in the 2021 boom, but afterwards they did not track profits closely.
3. **Regulatory Capital (Panel A):**
   Goldman Sachs, Morgan Stanley and JPMorgan kept Common Equity Tier 1 (CET1) capital ratios between **13.0% and 17.4%**, which is consistent with regulatory buffers (set by Federal Reserve CCAR stress tests) limiting how much capital these banks return.
4. **Pay Squeezed Margins at Advisory Boutiques (Panel B):**
   In the 2023 slowdown the boutiques' pay fell less than their revenue. Compensation expense ratios rose from 60% to 64% in the 2021 boom to 66% to 72% in 2023 (as much as 71.6% of revenue), and operating margins fell.
5. **Lagged Associations ($t \to t+1$):**
   Prior-year share repurchases showed almost no linear association with next-year return on equity for the banks in Panel A ($r = -0.049$), so buybacks did not predict how profitable the banks would be.

---

## 4. Empirical Methodology & Data Provenance

- **Primary Source Data:** I hand-collected the input figures from SEC Form 10-K filings on EDGAR. The provenance map lists where each one comes from.
- **Non-Causal Stance:** This study documents **empirical patterns and longitudinal associations** across firms; it does not claim to prove econometric causality.

---

## 5. Repository Structure

```text
strategic-capital-allocation-investment-banking/
├── README.md                      # Project overview and student research note
├── FINAL_PAPER.md                 # Complete research paper (Markdown)
├── FINAL_PAPER.pdf                # 20-page formatted research paper with embedded charts
├── FINAL_PAPER.docx               # Formatted Word manuscript
│
├── data/ (PHASE3 CSVs)            # Raw extracted observations from SEC 10-K filings
│   ├── PHASE3_RAW_DATA.csv        # Hand-collected balance sheet and income metrics
│   ├── PHASE3_DERIVED_DATA.csv    # Payout ratios, CET1 metrics, and compensation ratios
│   └── PHASE3_PROVENANCE_MAP.csv  # Page-by-page mapping to SEC Form 10-K filings
│
├── analysis/ (PHASE4 CSVs)        # Descriptive statistics, cross-firm tables, and lagged metrics
└── charts/ (PHASE4_CHARTS)        # High-resolution charts of revenues, distributions, and CET1 ratios
```

---

---

## 6. Research Methodology & Transparency Note
As an independent 12th-grade student researcher, I formulated the research question, collected and checked the SEC Form 10-K disclosures across all eight institutions, and conducted the comparative financial analysis. I used AI coding assistants to assist with data structuring, generating charts, and refining written drafts. All final empirical observations, interpretations, and conclusions are my own.

## 7. Citation

```bibtex
@misc{can2026capitalallocation,
  author       = {Ege Umut Can},
  title        = {Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020 to 2024},
  year         = {2026},
  school       = {FMV Işık High School, Istanbul},
  howpublished = {\url{https://github.com/ege211/strategic-capital-allocation-investment-banking}}
}
```

---

## 8. License

This project is licensed under the [MIT License](LICENSE).
