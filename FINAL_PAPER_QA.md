# Phase 6 Final Paper Forensic Quality Assurance Report

**Project Title**: Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024  
**Author**: Ege Can (12th-Grade Independent Student Researcher)  
**Date**: September 2026  
**Status**: 20-Point Forensic Audit Complete — PASS (20 / 20)  

---

## Executive Summary

This Quality Assurance report provides a complete forensic verification of the final integrated publication deliverables for Project 4:
- `FINAL_PAPER.md` (Markdown format, 6,755 prose words, 13 required academic sections)
- `FINAL_PAPER.docx` (Microsoft Word format, 2.1 MB, fully styled with embedded figures and tables)
- `FINAL_PAPER.pdf` (Adobe PDF format, 20 numbered pages, running headers, footers, and figures)
- `FINAL_PAPER_SOURCE_MAP.csv` (Cell-level provenance connecting 22 major empirical claims to Phase 3/4 sources)

All twenty audit checks mandated by the Phase 6 specification were evaluated against the frozen empirical datasets, the primary SEC Form 10-K source register, and the author's core interpretation framework. Every check achieved a **PASS** result.

---

## 20-Point Forensic Audit Checklist

| Check ID | Audit Criterion | Evaluation Scope & Evidence | Result |
| :--- | :--- | :--- | :---: |
| **CHECK_01** | **No new empirical observations** | Verified that no new data points, observations, or metrics were introduced. All data originate strictly from the 540 raw and 70 derived observations locked in Phase 3. | **PASS** |
| **CHECK_02** | **No changed numerical values** | All totals ($233.2B returned, $113.8B dividends, $119.3B repurchases), firm-level growth rates (GS +92.5%, MS +124.1%, JPM +16.5%, SF +208.0%), and CET1 ratios (13.1%–17.4% for GS/MS/JPM; 11.24% for SF) match Phase 4 exactly. | **PASS** |
| **CHECK_03** | **No changed correlations** | All Pearson and Spearman correlation coefficients in Table 8 and Section 7 match `PHASE4_CORRELATIONS.csv` exactly (Panel A repurchases $\to$ ROE: $r = -0.049$, $\rho = -0.035$; Panel B repurchases $\to$ margin: $r = -0.403$, $\rho = -0.385$; Panel B fee rev $\to$ op income: $r = +0.470$, $\rho = +0.503$). | **PASS** |
| **CHECK_04** | **No changed p-values** | All reported $p$-values match `PHASE4_CORRELATIONS.csv` exactly ($p = 0.858 / 0.897$ for Panel A repurchases $\to$ ROE; $p = 0.194 / 0.217$ for Panel B repurchases $\to$ margin; $p = 0.123 / 0.095$ for Panel B fee revenue $\to$ operating income). | **PASS** |
| **CHECK_05** | **No changed sample sizes** | Transition sample sizes ($N = 16$ for Panel A, $N = 12$ for Panel B) are preserved across all tables, charts, text references, and appendices. | **PASS** |
| **CHECK_06** | **No causal claims** | Text strictly uses observational language (`coincided with`, `was observed alongside`, `is associated with`). Zero occurrences of `caused`, `causes`, `led to`, `resulted in`, or `drove`. | **PASS** |
| **CHECK_07** | **No management-motive claims as fact** | No statements inferring executive intent as proven fact. Dividend stability and repurchase variation described strictly observationally. Zero occurrences of `management chose`, `management decided`, or `firms deliberately`. | **PASS** |
| **CHECK_08** | **No rankings** | No comparative ranking of firms or business models (`best`, `worst`, `top performer`, `superior allocator`). | **PASS** |
| **CHECK_09** | **No "best/worst/superior" conclusions** | Business model neutrality strictly maintained in Section 8 and Section 10. Both BHC and advisory models described as coherent structures designed for different financial activities. | **PASS** |
| **CHECK_10** | **Panel architecture preserved** | Panel A (GS, MS, JPM, SF) and Panel B (EVR, LAZ, MC) maintained as separate analytical panels throughout all analyses, tables, and discussions. | **PASS** |
| **CHECK_11** | **JEF remains sensitivity/context** | Jefferies Financial Group (`JEF`) evaluated strictly as a standalone sensitivity/context comparison due to its November 30 fiscal year-end and broker-dealer regulatory framework; never pooled into Panel A or Panel B. | **PASS** |
| **CHECK_12** | **Decision-making labelled as unobserved** | Conceptual chain (`Financial Conditions -> Decision-Making Considerations -> Capital-Allocation Decisions -> Financial Outputs`) is explicitly defined in Section 3 and Section 8 as an author-led interpretive hypothesis, with disclosure that internal deliberations are unobserved in SEC filings. | **PASS** |
| **CHECK_13** | **Small-N limitation disclosed** | Small sample sizes ($N = 16$ and $N = 12$) explicitly disclosed as exploratory in Abstract, Section 4.3, Section 7.4, Section 9 (Limitation 1), Section 10, and Appendix E. | **PASS** |
| **CHECK_14** | **2020–2024 limitation disclosed** | Five-year observation period and unique macroeconomic cycle (COVID shock, 2021 liquidity boom, 525 bps rate tightening) disclosed as non-generalizable to multi-decade secular trends in Section 9 (Limitations 2 and 3). | **PASS** |
| **CHECK_15** | **No fabricated citations** | References restricted strictly to verified primary SEC Form 10-K filings, Federal Reserve regulations (12 C.F.R. Parts 217 and 252), and Basel Committee publications. Zero synthetic or invented literature citations. | **PASS** |
| **CHECK_16** | **All major numerical claims traceable** | 100% of major empirical claims mapped directly to Phase 3/4 files and audited Form 10-K sections in `FINAL_PAPER_SOURCE_MAP.csv`. | **PASS** |
| **CHECK_17** | **No local filesystem paths in final outputs** | Confirmed 0 occurrences of local environment paths (e.g., local user directories) in `FINAL_PAPER.md`, `FINAL_PAPER.docx`, `FINAL_PAPER.pdf`, and `FINAL_PAPER_SOURCE_MAP.csv`. | **PASS** |
| **CHECK_18** | **Student voice remains accessible** | Tone throughout reflects an ambitious, intellectually rigorous, and modest 12th-grade student researcher (Ege Can). Confirmed 0 occurrences of graduate-level jargon (`empirical architecture`, `endogenous optimization`, `deterministic driver`, `capital-allocation mechanism`). | **PASS** |
| **CHECK_19** | **Phase 1–5 files untouched** | Confirmed that all Phase 1–5 files, raw data, derived data, descriptive stats, correlations, tables, charts, and discussion files remained 100% frozen and unmodified during Phase 6. | **PASS** |
| **CHECK_20** | **Final conclusion matches evidence** | Conclusion synthesizes findings around the four core questions, affirming the author's central insight (*"financial outputs cannot always be understood by looking at individual financial variables in isolation"*) within strict observational boundaries. | **PASS** |

---

## Detailed Check Verification Logs

### 1. Dataset & Numerical Immutability Verification (CHECK_01 – CHECK_05, CHECK_19)
- Phase 3 raw dataset (`PHASE3_RAW_DATA.csv`): 77,770 bytes, verified unchanged from 09:52:14.
- Phase 3 derived dataset (`PHASE3_DERIVED_DATA.csv`): 19,522 bytes, verified unchanged from 09:52:14.
- Phase 4 correlation dataset (`PHASE4_CORRELATIONS.csv`): 11,495 bytes, verified unchanged from 10:35:27.
- Phase 4 tables (`PHASE4_TABLES.md`): 21,229 bytes, verified unchanged from 10:35:31.
- All 18 chart assets in `PHASE4_CHARTS/`: verified intact and identical to Phase 4 outputs.

### 2. Semantic and Epistemic Audit (CHECK_06 – CHECK_09, CHECK_12, CHECK_18)
- Causal terminology scan: zero instances of causal verbs (`caused`, `drove`, `resulted in`, `led to`, `because X caused Y`).
- Intentionality scan: zero instances of unverified management motive assertions (`management chose`, `management decided`, `firms deliberately`).
- Evaluative scan: zero instances of subjective ranking terms (`best`, `worst`, `superior`, `more effective`).
- Decision-making framework: Sections 3, 5.3, 8.5, and 10 explicitly state that decision-making considerations (risk tolerance, talent retention, balance-sheet safety, liquidity needs, shareholder expectations) are hypothetical explanatory factors that are not directly observed or measured in SEC Form 10-K filings.

### 3. Sourcing and Traceability Audit (CHECK_15, CHECK_16, CHECK_17)
- `FINAL_PAPER_SOURCE_MAP.csv` documents 22 major empirical claims, cross-referencing statement IDs, exact figures, Phase 3/4 source files, table rows, and SEC accession numbers.
- File-path sanitization: Automated regex inspection confirmed zero local environment path leaks across all deliverables.

---

## Final QA Sign-Off

- **Audit Completion Timestamp**: September 2026
- **Total Audited Checks**: 20
- **Total Passed Checks**: 20
- **Total Failed Checks**: 0
- **Audit Verdict**: **PASS — 100% COMPLIANT**
