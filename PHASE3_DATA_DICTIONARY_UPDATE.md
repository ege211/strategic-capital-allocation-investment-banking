# Phase 3 Data Dictionary Update: Variable Structure & Hierarchy

**Project Title**: Strategic Capital Allocation in Investment Banking (2020–2024)  
**Author**: 12th-Grade Independent Student Research Project  
**Target Period**: Fiscal Years 2020, 2021, 2022, 2023, and 2024 strictly  
**Status**: Updated for Phase 3 Data Collection  

---

## 1. Overview of the Data Architecture

In this research project, I am investigating how major investment banking firms allocate their capital between business investments, capital buffers, and shareholder payouts, and how these decisions relate to their performance.

Because investment banks have different business models and regulatory rules, I organized the variables into three clear groups:
1. **Common GAAP Core**: 5 variables available across all firms from standard financial statements.
2. **Panel A (Bank Holding Companies)**: 8 core analytical variables + 3 supplementary descriptive variables.
3. **Panel B (Independent Advisory Boutiques)**: 7 core analytical variables + 4 supplementary descriptive variables.

Separating core analytical variables from supplementary descriptive variables keeps the dataset clean and manageable, which fits the realistic scope of a high-school student research project.

---

## 2. Common GAAP Core (5 Core Variables)

These 5 variables come directly from standard audited financial statements under U.S. GAAP and are comparable across all 8 firms:

| Variable Name | Display Name | Category | Unit | Accounting Source | Definition |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `net_revenue` | Total Net Revenues | Resources | USD Millions | Income Statement | Revenues net of interest expense; aggregate top line. |
| `investment_banking_revenue`| Investment Banking Fees | Resources | USD Millions | Income Statement / Note | Underwriting and financial advisory fees. |
| `dividends_paid` | Cash Dividends Paid | Shareholder Return | USD Millions | Cash Flows (Financing) | Cash dividends paid on common and preferred stock. |
| `share_repurchases` | Share Repurchases | Shareholder Return | USD Millions | Cash Flows (Financing) | Cash paid to repurchase common shares/treasury stock. |
| `total_cash_returned` | Total Cash Returned | Shareholder Return | USD Millions | Derived (`div + repurch`) | Sum of cash dividends and share repurchases. |

---

## 3. Panel A: Bank Holding Companies (`GS`, `MS`, `JPM`, `SF`)

Bank holding companies are large, balance-sheet-intensive financial institutions regulated by the Federal Reserve under Basel III capital rules.

### Core Analytical Variables (8 Variables)
1. `net_revenue` (Total revenues net of interest expense)
2. `investment_banking_revenue` (Advisory and underwriting fees)
3. `roe_or_rotce` (Return on common equity or return on tangible common equity)
4. `efficiency_or_overhead_ratio` (Non-interest operating expenses divided by net revenues)
5. `cet1_standardized` (Basel III Standardized Common Equity Tier 1 capital ratio)
6. `tier1_leverage_ratio` (Federal Reserve Tier 1 capital to average assets)
7. `dividends_paid` (Cash dividends paid)
8. `share_repurchases` (Common stock repurchased)

### Supplementary Descriptive Variables (3 Variables)
These variables provide useful context but are not forced into the primary statistical comparisons:
- `supplementary_leverage_ratio` (SLR): Basel III leverage ratio including off-balance-sheet items. Reported by G-SIBs (`GS`, `MS`, `JPM`). Stifel (`SF`) is a Category IV bank and is legally exempt from SLR, so it is marked `NOT_APPLICABLE`.
- `tangible_common_equity`: Common equity minus goodwill and intangible assets; measures tangible capital cushion.
- `technology_or_business_investment`: Operating expenses for communications, market data feeds, and IT infrastructure. Kept as supplementary because it represents operating expenses rather than total capital expenditures.

---

## 4. Panel B: Independent Advisory Boutiques (`EVR`, `LAZ`, `MC`)

Advisory boutiques are asset-light firms focused on financial advice (M&A, restructuring). They do not take customer deposits or maintain large trading balance sheets.

### Core Analytical Variables (7 Variables)
1. `net_revenue` (Total net advisory revenues)
2. `investment_banking_revenue` (Core advisory and underwriting revenue)
3. `compensation_expense` (Salary, bonus pool, and stock compensation)
4. `compensation_ratio` (Compensation expense divided by net revenue)
5. `operating_income` (Operating profit before taxes and partner allocations)
6. `operating_margin` (Operating income divided by net revenue)
7. `dividends_and_shareholder_distributions` (Cash dividends and partner distributions + share repurchases)

### Supplementary Descriptive Variables (4 Variables)
- `cash`: Unencumbered cash and cash equivalents held on the balance sheet.
- `debt`: Funded long-term debt (Evercore and Moelis have zero funded debt; Lazard carries senior notes).
- `net_cash_or_net_debt`: Cash minus funded debt; reflects the firm's net liquid cushion.
- `technology_or_business_investment_if_available`: Communications and market data expenses (reported by Evercore and Lazard; unavailable for Moelis, which bundles it into general expenses).

---

## 5. Extended / Sensitivity Firm: Jefferies (`JEF`)

Jefferies is kept in a separate **Sensitivity** category because:
1. It is a broker-dealer holding company (regulated under SEC Rule 15c3-1), not a bank holding company.
2. Its fiscal year ends on **November 30** rather than December 31.
3. During 2020–2022, it was transitioning away from legacy merchant-banking assets.

All available data for Jefferies was collected from its official Form 10-K filings, but it remains isolated so that it does not distort the findings of Panel A or Panel B.

---

## 6. Derived Variables & Calculation Rules

Every derived variable in the dataset is calculated using an explicit mathematical formula and links directly to verified raw observations:

1. **`total_cash_returned`**:
   - *Formula*: `dividends_paid + share_repurchases`
   - *Inputs*: `RAW_{ticker}_{year}_dividends_paid`, `RAW_{ticker}_{year}_share_repurchases`
   - *Unit*: USD Millions

2. **`operating_margin`** (for boutiques):
   - *Formula*: `operating_income / net_revenue * 100`
   - *Inputs*: `RAW_{ticker}_{year}_operating_income`, `RAW_{ticker}_{year}_net_revenue`
   - *Unit*: %

3. **`net_cash_or_net_debt`** (for boutiques):
   - *Formula*: `cash - debt`
   - *Inputs*: `RAW_{ticker}_{year}_cash`, `RAW_{ticker}_{year}_debt`
   - *Unit*: USD Millions

---

## 7. Status & Comparability Labels

To avoid confusion and prevent errors:
* `DIRECT`: Directly reported in the SEC Form 10-K.
* `DERIVED`: Calculated using an explicit formula from verified numbers.
* `UNAVAILABLE`: Not reported by the company (e.g., Moelis technology expense). Never replaced with zero.
* `NOT_APPLICABLE`: Does not apply under the company's regulatory rules (e.g., CET1 for boutiques, or SLR for Stifel). Never replaced with zero.
* `STRUCTURALLY_NON_COMPARABLE`: Reported, but the underlying business or accounting meaning is fundamentally different (e.g., bank cash vs boutique cash). Kept isolated from pooled comparisons.
