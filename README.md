# Strategic Capital Allocation in Investment Banking
### A Comparative Longitudinal Study of Major U.S. Firms (2020–2024)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Academic Level](https://img.shields.io/badge/Level-High%20School%20Student%20Research-blue.svg)](#)
[![Data Source](https://img.shields.io/badge/Data-SEC%20Form%2010--K%20Filings-green.svg)](https://www.sec.gov/edgar)

> **An independent high-school student research project analyzing how leading Wall Street investment banks and advisory boutiques allocated capital between balance-sheet retention, reinvestment, and shareholder distributions during periods of macroeconomic volatility.**

---

## 1. Student Researcher's Note & Motivation

**Author:** Ege Can  
**School:** FMV Özel Ispartakule Işık High School, Istanbul (Class of 2027)  
**Research Focus:** Corporate Finance, Capital Structure & Banking Regulation  

### Why I Undertook This Study:
When studying introductory economics and corporate finance, capital allocation is often taught through simple textbook formulas. Yet in the real financial world, executive leadership faces difficult trade-offs: *Should excess cash be returned to shareholders via buybacks and dividends, held on the balance sheet as a regulatory cushion, or reinvested into employee compensation and technology?*

Between 2020 and 2024, the global economy witnessed an unprecedented sequence of shocks: the initial COVID-19 pandemic shutdown and emergency stimulus (2020), an explosive boom in corporate mergers and IPOs (2021), followed by the steepest Federal Reserve interest-rate hiking cycle in four decades (2022–2023), and subsequent market stabilization (2024).

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

1. **$233.2 Billion in Shareholder Distributions:**
   Across the eight firms over the 2020–2024 period, a combined **$233.2 billion** was returned to equity holders ($113.8 billion in regular cash dividends and $119.3 billion in share repurchases).
2. **Dividends as a Stable Anchor vs. Cyclical Buybacks:**
   Regular cash dividends grew steadily across all firms, functioning as a non-discretionary baseline. In contrast, common share repurchases fluctuated widely, surging during peak profit years (2021) and pulling back when market deal-flow contracted (2022–2023).
3. **The Power of Regulatory Solvency (Panel A):**
   Large bank holding companies maintained strict Common Equity Tier 1 (CET1) capital ratios between **13.1% and 17.4%**, demonstrating how regulatory buffers (mandated by Federal Reserve CCAR stress tests) strictly condition capital return decisions.
4. **Compensation Flexibility in Advisory Boutiques (Panel B):**
   Independent boutiques operate with flexible cost structures: compensation expense ratios expanded from 60%–64% during the 2021 boom to 66%–72% during the 2023 deal drought, cushioning the firms during cyclical downturns without requiring large debt cushions.
5. **Lagged Associations ($t \to t+1$):**
   Prior-year share repurchases showed virtually zero linear association with next-year return on equity for large banks ($r = -0.049$), illustrating that capital distributions reflect cyclical timing rather than guaranteed forward operating performance.

---

## 4. Empirical Methodology & Data Provenance

- **100% Primary Source Data:** Every figure in the dataset was extracted directly from audited SEC Form 10-K filings filed with the U.S. Securities and Exchange Commission (EDGAR system).
- **Non-Causal Stance:** In keeping with rigorous student research, this study documents **empirical patterns and longitudinal associations** across firms; it does not claim to prove econometric causality.

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
As an independent 12th-grade student researcher, I formulated the research question, collected and verified the audited SEC Form 10-K disclosures across all eight institutions, and conducted the comparative financial analysis. I used AI coding assistants to assist with data structuring, generating charts, and refining written drafts. All final empirical observations, interpretations, and conclusions are my own.

## 7. Citation

```bibtex
@misc{can2026capitalallocation,
  author       = {Ege Can},
  title        = {Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms (2020--2024)},
  year         = {2026},
  school       = {FMV Işık High School},
  howpublished = {\url{https://github.com/ege211/strategic-capital-allocation-investment-banking}}
}
```

---

## 8. License

This project is licensed under the [MIT License](LICENSE).
