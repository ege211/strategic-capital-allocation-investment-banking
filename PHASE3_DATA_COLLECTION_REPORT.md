# Phase 3 Data Collection Report: Strategic Capital Allocation in Investment Banking (2020–2024)

**Project Title**: Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024  
**Author**: 12th-Grade Independent Student Research Project  
**Target Period**: Fiscal Years 2020, 2021, 2022, 2023, and 2024  
**Current Phase**: Phase 3 Complete (Data Collection and Source Documentation)  

---

## 1. What Was Collected

In this phase of my research project, I collected the actual financial numbers for eight major Wall Street investment banking and advisory firms over the five-year period from 2020 through 2024.

Rather than relying on commercial websites or summary databases, I collected observations directly from official annual reports (SEC Form 10-K filings). Collected observations were linked to SEC filings through the project provenance map. For each number, I recorded:
- The reported dollar amount or percentage.
- The company's original reporting terminology.
- The specific filing date, SEC accession number, and official EDGAR URL.
- The specific financial statement, footnote, or MD&A section where the number appears.
- Whether the number was directly reported or mathematically calculated (such as total cash returned to shareholders).

In total, I collected **540 raw observations** and calculated **70 derived observations** across the eight firms, backed by **40 primary Form 10-K filings**.

---

## 2. Which Firms Were Covered

The eight firms represent the major players in U.S. investment banking, but because they have very different business models, I organized them into two main panels and one separate sensitivity observation:

### Main Panel A: Bank Holding Companies (4 Firms)
1. **The Goldman Sachs Group, Inc. (`GS`)**: Global investment banking, trading, and asset management.
2. **Morgan Stanley (`MS`)**: Investment banking, institutional trading, and a massive wealth management franchise.
3. **JPMorgan Chase & Co. (`JPM`)**: Universal banking giant; I focused on firm-wide capital and its Commercial & Investment Bank (CIB) operations.
4. **Stifel Financial Corp. (`SF`)**: Mid-sized financial holding company with strong wealth management and middle-market investment banking.

### Main Panel B: Independent Advisory Boutiques (3 Firms)
5. **Evercore Inc. (`EVR`)**: Premier independent investment banking advisory firm.
6. **Lazard, Inc. (`LAZ`)**: Historic financial advisory and asset management house (converted to a U.S. C-Corporation in 2024).
7. **Moelis & Company (`MC`)**: Pure-play global advisory firm focused on M&A, restructuring, and capital structure advice.

### Sensitivity / Context Observation (1 Firm)
8. **Jefferies Financial Group Inc. (`JEF`)**: Full-service broker-dealer and investment bank. Jefferies is kept in a separate group because its fiscal year ends on November 30 (one month earlier than the others) and it is regulated as a broker-dealer rather than a bank holding company.

---

## 3. Which Years Were Covered

I collected data for exactly five fiscal years:
* **2020**: The onset of the COVID-19 pandemic, emergency Federal Reserve rate cuts to 0%, and market stimulus.
* **2021**: A historic boom year for investment banking, with record M&A activity, debt issuance, and tech IPOs.
* **2022**: The Federal Reserve's rapid 525-basis-point interest rate hiking cycle, causing debt and equity underwriting to decline sharply.
* **2023**: Continued advisory slowdown, regional banking stress (e.g., Silicon Valley Bank, First Republic), and low M&A completions.
* **2024**: Cyclical rebound in announced M&A, debt refinancing, and investment banking fees.

All firms are reported on their actual fiscal year-end (December 31 for seven firms, and November 30 for Jefferies). I did not collect any data from 2025 or 2026.

---

## 4. Main Variables

To make the study realistic and manageable for a student project, I focused on a small, clear set of variables rather than collecting hundreds of unneeded data points:

### A. Common Core Variables (Available for all 8 firms)
* **`net_revenue`**: Total net revenues (revenues after interest expense).
* **`investment_banking_revenue`**: Fees earned from advisory (M&A, restructuring) and underwriting (equity and debt).
* **`dividends_paid`**: Actual cash paid out for dividends during the year (from the Statement of Cash Flows).
* **`share_repurchases`**: Actual cash spent buying back common stock (from the Statement of Cash Flows).
* **`total_cash_returned`**: The sum of cash dividends and share repurchases (`dividends_paid + share_repurchases`).

### B. Bank Holding Company Core Variables (Panel A)
* **`roe_or_rotce`**: Return on common equity (ROE) and return on tangible common equity (ROTCE / ROTE).
* **`efficiency_or_overhead_ratio`**: Total operating expenses divided by net revenues (measures cost discipline).
* **`cet1_standardized`**: Common Equity Tier 1 capital ratio under Federal Reserve Basel III rules (the key measure of bank solvency).
* **`tier1_leverage_ratio`**: Tier 1 capital divided by average total assets.

### C. Advisory Boutique Core Variables (Panel B)
* **`compensation_expense`**: Total salary, incentive bonuses, and stock awards paid to bankers.
* **`compensation_ratio`**: Compensation expense divided by net revenue (the primary steering metric for advisory firms, usually 55%–70%).
* **`operating_income`**: Revenues minus operating expenses.
* **`operating_margin`**: Operating income divided by net revenue (measures operating profitability).
* **`dividends_and_shareholder_distributions`**: Cash returned to public shareholders and operating partners.

### D. Supplementary Descriptive Variables
I also gathered supplementary data that provides helpful context but will not be forced into the main statistical models:
* *For Banks*: Supplementary Leverage Ratio (SLR), Tangible Common Equity (TCE), and operating technology expenses.
* *For Boutiques*: Balance-sheet cash, long-term debt, and net cash/debt.

---

## 5. Main Sources

All data was collected directly from official first-party regulatory filings:
1. **SEC Form 10-K Annual Reports**: Retrieved via the SEC EDGAR system for each firm from FY 2020 through FY 2024.
2. **SEC XBRL Company Facts**: Used to verify exact tag names, filing dates, and numerical values against audited tables.
3. **Primary Document Links**: Collected observations were linked to SEC filings through the project provenance map, including official SEC EDGAR URLs and 20-digit accession numbers.

I did not use commercial financial websites (like Yahoo Finance, Macrotrends, or Statista) for any numbers.

---

## 6. Variables That Were Unavailable

Out of all 540 collected cells, only **5 observations were UNAVAILABLE**:
* **Moelis & Company (`MC`) Technology Expense**: Moelis does not report a separate line item for communications or technology expenses in its 10-K income statements or footnotes (it bundles these costs into general operating expenses).
* Rather than estimating or guessing a number, I followed the strict rule of this project and marked it **`UNAVAILABLE`**.

---

## 7. Variables That Were Not Comparable

Some metrics exist for some companies but cannot be compared across the entire group:
1. **Regulatory Capital for Boutiques (`cet1_standardized`, `tier1_leverage_ratio`, `supplementary_leverage_ratio`)**:
   - Advisory boutiques (Evercore, Lazard, Moelis) are not bank holding companies. They do not take customer deposits or hold commercial loans, so Federal Reserve Basel III capital rules do not apply to them.
   - These cells are explicitly marked **`NOT_APPLICABLE`** (and never set to zero).
2. **Supplementary Leverage Ratio (SLR) for Stifel (`SF`)**:
   - Stifel is a Category IV regional bank. Under Federal Reserve rules, Category IV banks are legally exempt from calculating or publishing an SLR ratio. This is marked **`NOT_APPLICABLE`**.
3. **Return on Equity (ROE) for Advisory Boutiques**:
   - Evercore and Moelis use partnership structures (Up-C partnerships) where partner equity is excluded from public common equity, making book ROE artificially inflated. Lazard also had historically depleted book equity from past partner distributions.
   - Therefore, ROE is marked **`STRUCTURALLY_NON_COMPARABLE`** for Panel B. Boutiques manage their business using operating margin and compensation ratios instead.
4. **Bank Cash and Debt vs Boutique Cash and Debt**:
   - Bank cash represents Federal Reserve reserve requirements and clearing deposits. Bank debt is used to fund trading inventory and loans.
   - In boutiques, cash represents corporate treasury reserves, and debt represents senior corporate borrowing. These serve completely different economic functions and are marked **`STRUCTURALLY_NON_COMPARABLE`** across panels.

---

## 8. Important Accounting Differences Discovered

During data collection, I noted several accounting differences:
1. **Overhead Ratio vs Efficiency Ratio**:
   - Goldman Sachs, Morgan Stanley, and Stifel report an "Efficiency Ratio" (non-interest expense / net revenue).
   - JPMorgan Chase calls this exact same metric the "Overhead Ratio".
   - In all cases, lower percentages indicate that operating expenses represent a smaller share of net revenue.
2. **Up-C Partnership Distributions**:
   - At Evercore and Moelis, founding partners hold operating partnership units alongside public Class A common shareholders. Cash returned to equity holders includes both corporate dividends and partnership distributions.
3. **Cash Flow vs Board Authorizations**:
   - Companies frequently announce multi-billion-dollar share buyback "authorizations" in press releases. However, authorizations can take years to execute or may never be used.
   - To be consistent and truthful, I recorded the actual cash dollars spent on share repurchases directly from the audited Statement of Cash Flows (Financing Activities).
4. **Temporary Pandemic SLR Relief**:
   - In 2020, the Federal Reserve temporarily allowed large banks to exclude U.S. Treasury bonds and central bank deposits from their leverage exposure. When this temporary relief expired on March 31, 2021, reported SLR ratios dropped slightly for Goldman Sachs, Morgan Stanley, and JPMorgan. This was a regulatory rule change, not a loss of capital.

---

## 9. Data Quality Checks (Basic QA)

Before completing Phase 3, I ran an automated 15-check verification program (`PHASE3_QA_RESULTS.csv`) to test the dataset:

| Check ID | Description | Result | Status |
| :--- | :--- | :---: | :---: |
| `CHECK_01` | All 8 firms have expected 2020–2024 coverage | **PASS** | Verified |
| `CHECK_02` | No 2025 or 2026 observations exist | **PASS** | Verified |
| `CHECK_03` | No unexplained blank numerical cells exist | **PASS** | Verified |
| `CHECK_04` | Unavailable values are explicitly labelled (Moelis tech) | **PASS** | Verified |
| `CHECK_05` | Not-applicable values are explicitly labelled | **PASS** | Verified |
| `CHECK_06` | No numerical value appears without a primary source record | **PASS** | Verified |
| `CHECK_07` | Every derived value has an explicit formula | **PASS** | Verified |
| `CHECK_08` | Every derived value references valid input observations | **PASS** | Verified |
| `CHECK_09` | No duplicate firm-year-variable observations | **PASS** | Verified |
| `CHECK_10` | Jefferies remains outside the two main panels | **PASS** | Verified |
| `CHECK_11` | Fiscal-year ends are preserved correctly (JEF Nov 30; others Dec 31)| **PASS** | Verified |
| `CHECK_12` | All SEC accession numbers and URLs are recorded | **PASS** | Verified |
| `CHECK_13` | No manually invented or guessed numbers appear | **PASS** | Verified |
| `CHECK_14` | Units are consistent across all variables ($ Millions or %) | **PASS** | Verified |
| `CHECK_15` | GAAP and non-GAAP metrics are clearly labelled | **PASS** | Verified |

All 15 quality checks passed with zero failures.

---

## 10. Remaining Limitations & Non-Causal Reminder

1. **Observational Study**: This study compares how firms allocated capital and how their businesses performed over time. It cannot prove that a specific payout policy *caused* a bank to perform better or worse.
2. **Cycle Effects**: The 2020–2024 window included extreme macroeconomic swings (COVID-19 stimulus, 0% interest rates, followed by 500+ basis points of rate hikes). Any relationship between capital allocation and performance must be interpreted in light of these industry-wide cycles.
3. **Jefferies Timing**: Jefferies' November 30 year-end means its results are reported one month ahead of the other firms. This is why it is kept in a separate sensitivity group.

---

## 11. Readiness for Phase 4

The raw data, provenance links, derived data, and quality checks are complete and verified:
- **`PHASE3_RAW_DATA.csv`**: 540 audited observations.
- **`PHASE3_PROVENANCE_MAP.csv`**: Collected observations were linked to SEC filings through the project provenance map.
- **`PHASE3_DERIVED_DATA.csv`**: 70 mathematical derivations with input tracking.
- **`PHASE3_SOURCE_REGISTER.csv`**: 40 verified Form 10-K filings.
- **`PHASE3_DATA_DICTIONARY_UPDATE.md`**: Student-friendly variable hierarchy.
- **`PHASE3_QA_RESULTS.csv`**: 15 passed automated tests.

Dataset ready for Phase 4 descriptive analysis.
