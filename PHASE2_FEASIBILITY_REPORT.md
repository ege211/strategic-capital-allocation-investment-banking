# Phase 2 Feasibility Report: Strategic Capital Allocation in Investment Banking (2020–2024)

**Project Title**: Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024  
**Author**: 12th-Grade Independent Student Research Project  
**Target Period**: Fiscal Years 2020, 2021, 2022, 2023, and 2024 strictly.  
**Phase Status**: Phase 1 **LOCKED** | Phase 2 **COMPLETE & VERIFIED**  
**Audit Standard**: Careful source-based analysis using primary SEC Form 10-K filings  
**Primary Filings Audited**: 40 Form 10-K Filings (8 Firms × 5 Fiscal Years)  

---

## Section A: Research Design Lock

### 1. Research Question
This student research project examines how major investment banking firms allocated their financial resources across business investments, capital buffers, and shareholder distributions during the 2020–2024 period, and how those decisions related to their subsequent financial performance.

* **Core Research Question**:
  > *"How do major investment-banking firms allocate capital between business investment, capital retention, and shareholder distributions, and how are these patterns associated with subsequent business performance?"*
* **Refined Analytical Question**:
  > *"To what extent are differences in capital retention and shareholder distribution associated with subsequent operating performance among major investment-banking firms?"*

### 2. Conceptual Framework
In corporate finance, earnings and operating cash flows can either be reinvested into the firm, held as capital reserves, or returned to shareholders:

```
                      +-------------------------------------------------------+
                      |                 FINANCIAL RESOURCES                   |
                      | (GAAP Net Revenues, Pre-Tax Cash Flow, Capital Base)  |
                      +-------------------------------------------------------+
                                                  │
                                                  ▼
                      +-------------------------------------------------------+
                      |             STRATEGIC CAPITAL ALLOCATION              |
                      +---------------------------┬---------------------------+
                                                  │
         ┌────────────────────────────────────────┼────────────────────────────────────────┐
         ▼                                        ▼                                        ▼
+───────────────────────────+    +───────────────────────────+    +───────────────────────────+
|    BUSINESS INVESTMENT    |    |     CAPITAL RETENTION     |    | SHAREHOLDER DISTRIBUTIONS |
| - Banker Compensation     |    | - Bank Regulatory CET1    |    | - Cash Dividends Paid     |
|   Pool (Human Capital)    |    |   & Tier 1 Leverage Ratios|    | - Share Repurchases       |
| - Technology & Market Data|    | - Corporate Cash Reserves |    |   (Treasury Stock Acq.)   |
|   Operating Expenses      |    |   (Boutique Liquidity)    |    |                           |
+───────────────────────────+    +───────────────────────────+    +───────────────────────────+
         │                                        │                                        │
         └────────────────────────────────────────┼────────────────────────────────────────┘
                                                  │
                                                  ▼
                      +-------------------------------------------------------+
                      |            SUBSEQUENT BUSINESS PERFORMANCE            |
                      |  - Return on Tangible Common Equity (ROTCE / ROTE)    |
                      |  - Operating Margin & Overhead Efficiency             |
                      |  - Investment Banking Revenues / Fees                 |
                      +-------------------------------------------------------+
```

### 3. Non-Causal Research Stance
Because this is an observational study of company financial statements without an experimental setup:
* I avoid words like *"causes"*, *"drives"*, *"impacts"*, or *"proves"*.
* I use careful observational language such as *"associated with"*, *"co-moved with"*, *"longitudinal comparison"*, and *"subsequent performance"*.

---

## Section B: Panel Architecture

In Phase 0, I discovered that combining diversified universal bank holding companies (BHCs) and independent advisory boutiques into a single table created important comparability problems. Their business models, balance sheets, and regulatory rules are completely different, so putting them in one simple comparison would make direct comparison difficult and misleading.

Therefore, I organized the project into two distinct main panels, plus one separate sensitivity observation:

```
┌─────────────────────────────────────────────────────────────────────────────────────────────┐
│                                 TOTAL CANDIDATE UNIVERSE (8 FIRMS)                          │
└──────────────────────────────────────────────┬──────────────────────────────────────────────┘
                                               │
             ┌─────────────────────────────────┼─────────────────────────────────┐
             ▼                                 ▼                                 ▼
┌─────────────────────────┐       ┌─────────────────────────┐       ┌─────────────────────────┐
│         PANEL A         │       │         PANEL B         │       │       SENSITIVITY       │
│  Regulated Bank Holding │       │   Independent Advisory  │       │       Quarantined       │
│        Companies        │       │        Boutiques        │       │      Observation        │
│      (4 Institutions)   │       │     (3 Institutions)    │       │     (1 Institution)     │
├─────────────────────────┤       ├─────────────────────────┤       ├─────────────────────────┤
│ • Goldman Sachs (GS)    │       │ • Evercore (EVR)        │       │ • Jefferies (JEF)       │
│ • Morgan Stanley (MS)   │       │ • Lazard (LAZ)          │       │                         │
│ • JPMorgan Chase (JPM)  │       │ • Moelis & Co. (MC)     │       │                         │
│ • Stifel Financial (SF) │       │                         │       │                         │
└─────────────────────────┘       └─────────────────────────┘       └─────────────────────────┘
             │                                 │                                 │
             └─────────────────────────────────┼─────────────────────────────────┘
                                               │
                                               ▼
                      ┌─────────────────────────────────────────────────┐
                      │              COMMON GAAP-CORE OVERLAY           │
                      │  - Total Net Revenues                           │
                      │  - Investment Banking Revenues / Fees           │
                      │  - Cash Dividends Paid                          │
                      │  - Cash Share Repurchases                       │
                      │  - Total Cash Returned to Shareholders          │
                      └─────────────────────────────────────────────────┘
```

### 1. Panel A: Regulated Bank Holding Companies (`GS`, `MS`, `JPM`, `SF`)
* **Regulatory Rules**: Regulated by the Federal Reserve under Basel III capital requirements and annual stress testing.
* **Business Model**: Large balance sheets with customer deposits, wholesale funding, and trading inventory.
* **Firm Differences**:
  * `GS`, `MS`, and `JPM` are Category I Global Systemically Important Banks (G-SIBs). They have the strictest capital requirements, including public Supplementary Leverage Ratio (SLR) buffers.
  * `SF` (Stifel Financial) is a Category IV regional financial holding company. It uses the Basel III Standardized Approach and is legally exempt from SLR requirements.

### 2. Panel B: Independent Advisory Boutiques (`EVR`, `LAZ`, `MC`)
* **Business Model**: Asset-light advisory firms that focus on M&A and restructuring advice. They do not hold customer deposits or massive trading portfolios.
* **Capital Allocation**: Their biggest allocation decision is the annual compensation pool for bankers (typically 55% to 70% of revenues). Cash left over is returned to shareholders through dividends and share buybacks.
* **Why Bank Metrics Don't Apply**: They are not bank holding companies, so regulatory ratios like CET1 and SLR are marked `NOT_APPLICABLE`. Furthermore, their partnership structures (Up-C partnerships for EVR and MC) and legacy capital structures (LAZ) distort standard book equity, making GAAP ROE structurally non-comparable.

### 3. Extended / Sensitivity Observation: Jefferies Financial Group (`JEF`)
* **Why Kept Separate**: Jefferies has a broker-dealer holding company structure (regulated under SEC Rule 15c3-1 rather than Federal Reserve bank rules), and its fiscal year ends on **November 30** (a 30-day reporting mismatch with the December 31 universe).
* **Role**: Kept separate as a sensitivity check so it does not distort Panel A or Panel B.

---

## Section C: Variable Structure & Counts

To ensure full consistency across all documentation, the variables are structured into core analytical variables and supplementary descriptive variables:

### 1. Common GAAP Core (5 Core Variables across all 8 firms)
These 5 variables are directly reported under standard U.S. GAAP across all firms:
1. `net_revenue`
2. `investment_banking_revenue`
3. `dividends_paid`
4. `share_repurchases`
5. `total_cash_returned` (Derived: `dividends_paid + share_repurchases`)

### 2. Panel A — Bank Holding Companies (8 Core + 3 Supplementary)
* **8 Core Analytical Variables**:
  1. `net_revenue`
  2. `investment_banking_revenue`
  3. `roe_or_rotce`
  4. `efficiency_or_overhead_ratio`
  5. `cet1_standardized`
  6. `tier1_leverage_ratio`
  7. `dividends_paid`
  8. `share_repurchases`
* **3 Supplementary Descriptive Variables**:
  - `supplementary_leverage_ratio` (reported by GS, MS, JPM; SF is exempt)
  - `tangible_common_equity`
  - `technology_or_business_investment` (operating tech expenses)

### 3. Panel B — Advisory Boutiques (7 Core + 4 Supplementary)
* **7 Core Analytical Variables**:
  1. `net_revenue`
  2. `investment_banking_revenue`
  3. `compensation_expense`
  4. `compensation_ratio`
  5. `operating_income`
  6. `operating_margin`
  7. `dividends_and_shareholder_distributions` (cash dividends + share repurchases)
* **4 Supplementary Descriptive Variables**:
  - `cash`
  - `debt`
  - `net_cash_or_net_debt`
  - `technology_or_business_investment_if_available`

*(Note: Supplementary variables provide helpful descriptive context, but they will not be forced into the main statistical models).*

---

## Section D: Source Hierarchy & Provenance Standards

### 1. Primary Sources
To ensure high research quality, all data comes from official regulatory filings:
1. **SEC Form 10-K Annual Reports**: The audited annual reports filed with the SEC.
2. **SEC XBRL Company Facts**: Official machine-readable data tags from SEC filings.
3. **Official First-Party Annual Reports & Shareholder Letters**: Used for segment descriptions and non-GAAP reconciliations.

### 2. Excluded Sources
I do not use third-party financial websites (like Yahoo Finance, Macrotrends, or Statista) as data sources because they often round numbers, adjust historical figures without explanation, or mix up fiscal year dates.

### 3. Verification of Source Register (`PHASE2_SOURCE_REGISTER.csv`)
All 40 Form 10-K filings across the 8 firms for the 5 years (2020–2024) have been verified with exact SEC accession numbers and official SEC EDGAR URLs.

---

## Section E: Firm-by-Firm Source Coverage

The cell-level source map (`PHASE2_SOURCE_MAP.csv`) covers all 880 firm-year-variable cells (8 firms × 5 years × 22 total tracked variables). Here is the breakdown across all 8 firms:

| Firm | Ticker | Panel | Period End | Total Cells | Directly Reported | Derived | Not Applicable | Structurally Non-Comparable | Unavailable |
| :--- | :--- | :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| Goldman Sachs | `GS` | Panel A | 12-31 | 110 | 65 | 10 | 15 | 20 | 0 |
| Morgan Stanley | `MS` | Panel A | 12-31 | 110 | 65 | 10 | 15 | 20 | 0 |
| JPMorgan Chase | `JPM` | Panel A | 12-31 | 110 | 65 | 10 | 15 | 20 | 0 |
| Stifel Financial | `SF` | Panel A | 12-31 | 110 | 60 | 10 | 20 | 20 | 0 |
| Evercore | `EVR` | Panel B | 12-31 | 110 | 55 | 15 | 35 | 5 | 0 |
| Lazard | `LAZ` | Panel B | 12-31 | 110 | 55 | 15 | 35 | 5 | 0 |
| Moelis & Co. | `MC` | Panel B | 12-31 | 110 | 50 | 15 | 35 | 5 | 5 |
| Jefferies | `JEF` | Sensitivity | 11-30 | 110 | 60 | 10 | 20 | 20 | 0 |
| **Total Universe** | **8 Firms** | — | — | **880** | **475** | **95** | **190** | **115** | **5** |

### Individual Firm Notes
1. **Goldman Sachs (`GS`)**: All BHC metrics are reported in Item 7 and Item 8. Standardized CET1, Tier 1 leverage, and SLR are clearly stated.
2. **Morgan Stanley (`MS`)**: Clean disclosures across all years. Wealth Management and Investment Management segments provide context for firm-wide overhead.
3. **JPMorgan Chase (`JPM`)**: Uses the term "Overhead Ratio" rather than "Efficiency Ratio". ROTCE, CET1, and SLR are reported consistently in Item 7.
4. **Stifel Financial (`SF`)**: Category IV bank; reports Basel III Standardized CET1 and Tier 1 leverage, but is exempt from SLR. Reports ROTE and efficiency ratio.
5. **Evercore (`EVR`)**: Clean boutique reporting. Zero funded debt reported. Discloses communications and information technology operating expenses.
6. **Lazard (`LAZ`)**: Reports compensation ratio, operating income, cash, and senior notes debt. Discloses information technology and market data expenses.
7. **Moelis & Company (`MC`)**: Discloses compensation ratio, operating income, and cash, but bundles technology expense into other expenses (marked `UNAVAILABLE` for tech expense).
8. **Jefferies (`JEF`)**: Complete coverage in 10-K filings; November 30 fiscal year-end preserved; kept in sensitivity analysis.

---

## Section F: Cross-Firm Comparability

### 1. Universal GAAP Items
Top-line revenues, investment banking fees, cash dividends paid, and share repurchases are directly comparable across all 8 firms because they follow standard U.S. GAAP definitions from the audited income and cash flow statements.

### 2. Bank Capital vs Boutique Liquidity
* Bank holding companies measure capital retention through regulatory capital ratios (CET1, Tier 1 leverage, SLR) enforced by the Federal Reserve. Bank cash represents reserve requirements and clearing deposits.
* Advisory boutiques measure capital retention through unencumbered cash and short-term investments on their balance sheet.

### 3. Overhead Ratio vs Compensation Ratio
* Banks have heavy non-personnel overhead (technology infrastructure, compliance, office networks) and manage to an **Overhead / Efficiency Ratio** (non-interest expenses / net revenues), typically around 60% to 75%.
* Boutiques have minimal physical assets and manage to a **Compensation Ratio** (compensation / net revenues), typically targeting 55% to 65%. These should not be directly combined.

---

## Section G: Known Structural Breaks (2020–2024)

Several real-world events occurred between 2020 and 2024 that must be remembered when analyzing the numbers:
1. **The 2020–2021 M&A and Underwriting Boom**: Low interest rates and government stimulus led to record investment banking revenues and high return metrics across Wall Street.
2. **The 2022–2023 Rate Hike Slowdown**: The Federal Reserve raised interest rates by over 500 basis points, causing IPO and debt underwriting activity to drop sharply.
3. **Expiration of Temporary SLR Relief (March 31, 2021)**: In 2020, the Fed temporarily let banks exclude U.S. Treasuries and deposits at the Fed from their leverage calculations. When this expired in March 2021, reported SLR ratios dropped slightly for GS, MS, and JPM.
4. **Major Acquisitions and Conversions**:
   * Morgan Stanley acquired E*TRADE (October 2020) and Eaton Vance (March 2021).
   * Jefferies spun off Vitesse Energy in 2022 and sold legacy merchant-banking assets.
   * Lazard converted from a Bermuda partnership to a U.S. C-Corporation on January 1, 2024.

---

## Section H: Variables Requiring Quarantine

1. **Technology Outlays**: Disclosed numbers represent ongoing operating expenses (market data feeds, communications, cloud computing run-rate) rather than total capitalized investment. Furthermore, Moelis does not report it separately. It is kept as supplementary descriptive data only.
2. **ROE for Boutiques**: Distorted by partnership equity accounting (Up-C) and legacy negative equity. Marked `STRUCTURALLY_NON_COMPARABLE` for Panel B.
3. **Wholesale Debt and Bank Cash**: Bank debt funds trading inventory and loan portfolios, whereas boutique cash represents corporate liquidity reserves. Kept separate.
4. **Jefferies (`JEF`) Data**: Maintained as an isolated sensitivity layer due to regulatory status and its November 30 fiscal year-end.

---

## Section I: Variables Eligible for Phase 3 Data Collection

The core dataset is clean and manageable:

### Group 1: Universal Common Core (All 8 Firms × 5 Years = 40 Firm-Years)
1. `net_revenue`
2. `investment_banking_revenue`
3. `dividends_paid`
4. `share_repurchases`
5. `total_cash_returned` (Derived)

### Group 2: Panel A Regulated BHCs (`GS`, `MS`, `JPM`, `SF` × 5 Years = 20 Firm-Years)
1. `net_revenue`
2. `investment_banking_revenue`
3. `roe_or_rotce`
4. `efficiency_or_overhead_ratio`
5. `cet1_standardized`
6. `tier1_leverage_ratio`
7. `dividends_paid`
8. `share_repurchases`
*(Plus 3 supplementary variables: `supplementary_leverage_ratio`, `tangible_common_equity`, `technology_or_business_investment`).*

### Group 3: Panel B Advisory Boutiques (`EVR`, `LAZ`, `MC` × 5 Years = 15 Firm-Years)
1. `net_revenue`
2. `investment_banking_revenue`
3. `compensation_expense`
4. `compensation_ratio`
5. `operating_income`
6. `operating_margin`
7. `dividends_and_shareholder_distributions`
*(Plus 4 supplementary variables: `cash`, `debt`, `net_cash_or_net_debt`, `technology_or_business_investment_if_available`).*

---

## Section J: Remaining Limitations & Verification Verdict

1. **Moelis Technology Data**: Moelis does not report technology expense separately. Rather than estimating or guessing, I mark this variable as `UNAVAILABLE` for Moelis.
2. **November 30 Year-End**: Jefferies has a one-month reporting difference from the other firms, which is why it is kept as a separate sensitivity observation.
3. **Readiness Verdict**: The data dictionary, source register, and source map are fully verified, and all automated checks have passed. The project is ready for Phase 3 primary-source data collection.
