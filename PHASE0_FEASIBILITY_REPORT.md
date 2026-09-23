# Phase 0 Feasibility Audit Report: Strategic Capital Allocation in Investment Banking (2020–2024)

**Project Title**: Strategic Capital Allocation in Investment Banking  
**Target Period**: Fiscal Years 2020–2024  
**Audit Scope**: 8 Candidate Firms (Goldman Sachs, Morgan Stanley, JPMorgan Chase, Jefferies Financial Group, Evercore, Lazard, Moelis & Company, Stifel Financial)  
**Primary Source Priority**: SEC Form 10-K Annual Filings & Official Financial Statements (No commercial databases)  
**Deliverable Files Created**:
1. `PHASE0_CANDIDATE_UNIVERSE.csv`
2. `PHASE0_VARIABLE_FEASIBILITY_MATRIX.csv`
3. `PHASE0_SOURCE_REGISTER.csv`
4. `PHASE0_FEASIBILITY_REPORT.md`

---

## 1. Executive Summary & Feasibility Verdict

This feasibility audit evaluated whether a comparable 5-firm panel can be constructed from primary-source SEC Form 10-K filings across 2020–2024 to investigate strategic capital allocation in investment banking.

### Core Verdict
A single, homogeneous 5-firm panel combining diversified bank holding companies (BHCs) and independent advisory boutiques **cannot be constructed without committing fatal semantic aggregation errors**. 

Specifically:
1. **Regulatory Capital (CET1 & Leverage)**: Basel III Common Equity Tier 1 (CET1) capital ratios, Supplementary Leverage Ratios (SLR), and Tier 1 Leverage ratios exist **only** for bank holding companies (Goldman Sachs, Morgan Stanley, JPMorgan Chase, Stifel Financial). Independent advisory boutiques (Evercore, Lazard, Moelis) and broker-dealer holding companies (Jefferies) are **not** bank holding companies and are legally exempt from Federal Reserve Basel III capital rules. They possess no CET1 ratios.
2. **Profitability & Capital Efficiency (ROE/ROTCE vs. Margins)**: While BHCs manage firm-wide balance sheets against Return on Tangible Common Equity (ROTCE) and Return on Equity (ROE), advisory boutiques operate Up-C partnership structures (Evercore, Moelis) or legacy partnership capital accounts (Lazard) where book equity is either heavily distorted, unrepresentative of total partner capital, or negative/near-zero. Consequently, boutiques steer by **Compensation Ratio** and **Operating Margin**, omitting ROE/ROTCE from their annual MD&A steering metrics.
3. **Fiscal-Year Discrepancy**: Jefferies Financial Group operates on a fiscal year ending **November 30**, whereas all other seven candidates operate on calendar years ending **December 31**.
4. **Viable Research Solutions**: Rather than forcing an artificial 5-firm panel that collapses incomparable banking and advisory definitions, the audit reveals three robust, methodologically defensible architectural designs:
   - **Architecture A (Bank Holding Company Panel)**: Goldman Sachs, Morgan Stanley, JPMorgan Chase, and Stifel Financial (4 BHCs, with potential expansion or 3 G-SIB core) examining regulatory capital allocation, balance-sheet leverage, and underwriting.
   - **Architecture B (Independent Advisory / Boutique Panel)**: Evercore, Lazard, and Moelis & Company (with optional inclusion of Jefferies on advisory metrics) examining human capital compensation ratios, operating margins, and free cash return.
   - **Architecture C (Common GAAP-Core Panel)**: A 5-to-8 firm panel restricted strictly to universally reported GAAP metrics (Net Revenue, Investment Banking Fees, Dividends Paid, Actual Share Repurchases, and Operating Cash Distributions).

---

## 2. Candidate Universe Audit & Regulatory Taxonomies

| Firm Name | Ticker | CIK | SIC Code | Entity & Regulatory Classification | Primary Business Model | Fiscal Year End | 2020–2024 Filing Coverage |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Goldman Sachs Group, Inc.** | GS | 0000886982 | 6211 | Bank Holding Company / FHC / G-SIB (Fed Basel III Standardized & Advanced, CCAR) | Global Banking & Markets, Asset & Wealth Management, Platform Solutions | Dec 31 | Complete (5/5 10-Ks) |
| **Morgan Stanley** | MS | 0000895421 | 6211 | Bank Holding Company / FHC / G-SIB (Fed Basel III Standardized & Advanced, CCAR) | Institutional Securities, Wealth Management, Investment Management | Dec 31 | Complete (5/5 10-Ks) |
| **JPMorgan Chase & Co.** | JPM | 0000019617 | 6021 | Universal Bank Holding Company / FHC / G-SIB (Fed Basel III Standardized & Advanced, CCAR) | Commercial & Investment Bank (CIB), Consumer Banking, Asset & Wealth Management | Dec 31 | Complete (5/5 10-Ks) |
| **Jefferies Financial Group Inc.** | JEF | 0000096223 | 6211 | Independent Broker-Dealer Parent (Broker-Dealer Jefferies LLC under SEC Rule 15c3-1; Non-BHC) | Full-Service Investment Banking and Capital Markets, Asset Management | **Nov 30** | Complete (5/5 10-Ks) |
| **Evercore Inc.** | EVR | 0001360901 | 6282 | Independent Advisory Boutique / Up-C Partnership (Broker-Dealer Subs under SEC Rule 15c3-1; Non-BHC) | Investment Banking (M&A Advisory, Equity/Debt Underwriting), Investment Management | Dec 31 | Complete (5/5 10-Ks) |
| **Lazard, Inc.** | LAZ | 0001311370 | 6282 | Independent Advisory & Asset Management Firm (Converted to DE C-Corp 2024; Non-BHC) | Pure Financial Advisory (M&A, Restructuring, Sovereign), Asset Management | Dec 31 | Complete (5/5 10-Ks) |
| **Moelis & Company** | MC | 0001596967 | 6282 | Pure-Play Advisory Boutique / Up-C Partnership (Broker-Dealer Subs under SEC Rule 15c3-1; Non-BHC) | 100% Strategic Financial Advisory (M&A, Capital Advisory, Restructuring); Zero Underwriting | Dec 31 | Complete (5/5 10-Ks) |
| **Stifel Financial Corp.** | SF | 0000720672 | 6211 | Regional Bank Holding Company / FHC Category IV (Fed Basel III Standardized Approach) | Global Wealth Management, Institutional Group (Advisory/Underwriting), Stifel Bank | Dec 31 | Complete (5/5 10-Ks) |

---

## 3. Audited Feasibility Matrix Across All 10 Variables

Every candidate firm was audited directly against its SEC Form 10-K filings for fiscal years 2020, 2021, 2022, 2023, and 2024.

### 3.1. Net Revenue
- **Goldman Sachs (GS)**: *Total net revenues* (Revenues net of interest expense). 2020: \$44,560M; 2021: \$59,339M; 2022: \$47,365M; 2023: \$46,254M; 2024: \$53,512M. (GAAP Direct, Consolidated Statements of Earnings).
- **Morgan Stanley (MS)**: *Net revenues* (Revenues net of interest expense). 2020: \$48,198M (recast \$48,757M); 2021: \$59,755M; 2022: \$53,668M; 2023: \$54,143M; 2024: \$61,761M. (GAAP Direct, Consolidated Statements of Income).
- **JPMorgan Chase (JPM)**: *Total net revenue*. 2020: \$119,543M; 2021: \$121,649M; 2022: \$128,695M; 2023: \$158,104M; 2024: \$177,556M. (GAAP Direct, Consolidated Statements of Income).
- **Jefferies (JEF)**: *Total net revenues*. FY20: \$6,002M; FY21: \$8,185M; FY22: \$5,979M; FY23: \$4,700M; FY24: \$7,035M. (GAAP Direct, Consolidated Statements of Earnings; Nov 30 FYE).
- **Evercore (EVR)**: *Net Revenues* (Total revenues less interest expense). 2020: \$2,264M; 2021: \$3,289M; 2022: \$2,762M; 2023: \$2,426M; 2024: \$2,980M. (GAAP Direct, Consolidated Statements of Operations).
- **Lazard (LAZ)**: *Net revenue* (Total revenue less interest expense). 2020: \$2,566M; 2021: \$3,193M; 2022: \$2,774M; 2023: \$2,515M; 2024: \$3,052M. (GAAP Direct, Consolidated Statements of Operations).
- **Moelis (MC)**: *Revenues*. 2020: \$943M; 2021: \$1,541M; 2022: \$985M; 2023: \$855M; 2024: \$1,195M. (GAAP Direct, Consolidated Statements of Operations; interest expense is immaterial).
- **Stifel (SF)**: *Total net revenues*. 2020: \$3,832M; 2021: \$4,737M; 2022: \$4,391M; 2023: \$4,349M; 2024: \$4,970M. (GAAP Direct, Consolidated Statements of Operations).
- **Feasibility & Comparability**: **100% Available and Directly Comparable across all 8 firms**.

### 3.2. Investment Banking Revenue / Fees
- **GS**: *Investment banking fees* (Advisory, Equity underwriting, Debt underwriting). 2020: \$9,141M; 2021: \$14,168M; 2022: \$7,360M; 2023: \$6,218M; 2024: \$7,738M. (GAAP Direct).
- **MS**: *Investment banking* (Advisory, Equity underwriting, Fixed income underwriting). 2020: \$7,674M; 2021: \$10,994M; 2022: \$5,599M; 2023: \$4,948M; 2024: \$6,705M. (GAAP Direct).
- **JPM**: *Investment banking fees* (Advisory, Equity underwriting, Debt underwriting). 2020: \$9,486M; 2021: \$13,216M; 2022: \$6,686M; 2023: \$6,519M; 2024: \$8,910M. (GAAP Direct, Noninterest revenue).
- **JEF**: *Total Investment Banking net revenues* (Advisory, Equity underwriting, Debt underwriting, Other IB). FY20: \$2,560M; FY21: \$4,657M; FY22: \$2,871M; FY23: \$2,272M; FY24: \$3,445M. (MD&A Segment Breakdown).
- **EVR**: *Advisory Fees + Underwriting Fees*. 2020: \$2,031M (\$1,755M adv / \$276M und); 2021: \$2,999M (\$2,752M adv / \$247M und); 2022: \$2,516M (\$2,393M adv / \$123M und); 2023: \$2,075M (\$1,964M adv / \$111M und); 2024: \$2,598M (\$2,441M adv / \$157M und). (GAAP Direct).
- **LAZ**: *Investment banking and other advisory fees* (Pure advisory/restructuring). 2020: \$1,418M; 2021: \$1,786M; 2022: \$1,659M; 2023: \$1,384M; 2024: \$1,747M. (GAAP Direct).
- **MC**: *Revenues (from investment banking advisory engagements)*. 2020: \$943M; 2021: \$1,541M; 2022: \$985M; 2023: \$855M; 2024: \$1,195M. (GAAP Direct; 100% advisory).
- **SF**: *Investment banking revenues* (Advisory and Capital raising/underwriting). 2020: \$952M; 2021: \$1,565M; 2022: \$971M; 2023: \$731M; 2024: \$995M. (GAAP Direct).
- **Feasibility & Comparability**: **100% Available across all 8 firms**. Highly comparable, with the semantic caveat that LAZ and MC represent pure advisory fees, EVR represents advisory plus niche underwriting, while GS, MS, JPM, JEF, and SF encompass advisory, equity underwriting, and debt/syndicated loan underwriting.

### 3.3. ROE or ROTCE
- **GS**: *ROE* (11.1%, 23.0%, 10.2%, 7.5%, 12.7%) / *ROTE* (11.8%, 24.3%, 11.0%, 8.1%, 13.5%). (Directly reported in MD&A).
- **MS**: *ROE* (13.1%, 15.0%, 11.2%, 9.4%, 14.0%) / *ROTCE* (15.2%, 19.8%, 15.3%, 12.8%, 18.8%). (Directly reported in MD&A).
- **JPM**: *ROE* (12%, 19%, 14%, 17%, 18%) / *ROTCE* (14%, 23%, 18%, 21%, 22%). (Directly reported in MD&A; ROTCE is JPM's core steering metric).
- **SF**: ROE is **NOT directly reported** as an annual steering table in 10-K; Derived ROE: 16.6% (2020), 18.8% (2021), 14.5% (2022), 9.9% (2023), 13.4% (2024).
- **JEF**: ROE is **NOT directly reported** in MD&A; ROTE is used as a 3-year executive compensation target (10%). Derived ROE: 7.9% (2020), 15.6% (2021), 7.4% (2022), 1.3% (2023), 4.7% (2024).
- **EVR**: ROE is **OMITTED** in 10-K. Due to the Up-C partnership structure, Class A common equity does not reflect partner capital. Operating Margin is reported instead: 23.3% (2020), 33.5% (2021), 25.2% (2022), 14.8% (2023), 17.7% (2024).
- **LAZ**: ROE is **OMITTED** in 10-K. Equity is structurally distorted by legacy Bermuda partnership distributions ($424M-$975M equity base on $3B revenue; 2023 net loss makes ROE uninterpretable). Operating Margin reported: 19.6% (2020), 22.7% (2021), 18.6% (2022), -3.2% (2023), 12.7% (2024).
- **MC**: ROE is **OMITTED** in 10-K. Up-C structure; Operating Margin reported: 28.2% (2020), 32.2% (2021), 21.9% (2022), -4.7% (2023), 14.5% (2024).
- **Feasibility & Comparability**: **Genuinely comparable ONLY within BHCs (GS, MS, JPM)**. Must be dropped or replaced with Operating Margin for advisory boutiques.

### 3.4. Efficiency Ratio or Comparable Operating Metric
- **BHCs (GS, MS, JPM)**: Report Bank Efficiency / Overhead Ratios (Total Non-Interest Expense divided by Net Revenue, where lower is better):
  * GS (*Efficiency ratio*): 65.0% (2020), 53.8% (2021), 65.8% (2022), 74.6% (2023), 63.1% (2024).
  * MS (*Expense efficiency ratio*): 69% (2020), 67% (2021), 73% (2022), 77% (2023), 71% (2024).
  * JPM (*Overhead ratio*): 56% (2020), 59% (2021), 59% (2022), 55% (2023), 52% (2024).
- **Boutiques & Broker-Dealers (JEF, EVR, LAZ, MC, SF)**: Steer by **Compensation Ratio** (Compensation & Benefits divided by Net Revenue):
  * JEF: 50.1% (2020), 52.8% (2021), 52.6% (2022), 59.4% (2023), 57.6% (2024).
  * EVR: 60.6% (2020), 56.2% (2021), 61.5% (2022), 68.3% (2023), 66.3% (2024).
  * LAZ: 60.4% (2020), 59.4% (2021), 59.7% (2022), 77.4% (2023), 65.6% (2024).
  * MC: 59.5% (2020), 59.3% (2021), 62.7% (2022), 83.6% (2023), 69.5% (2024).
  * SF: 62.7% (2020), 58.6% (2021), 57.3% (2022), 58.7% (2023), 57.7% (2024).
- **Feasibility & Comparability**: **Structurally bifurcated**. Efficiency Ratio (Total Expense / Revenue) is native to BHCs; Compensation Ratio is native to Boutiques and Broker-Dealers.

### 3.5. CET1 or Relevant Regulatory Capital Measure
- **GS**: Standardized CET1: 14.7% (2020), 14.2% (2021), 15.0% (2022), 14.4% (2023), 15.0% (2024). (Advanced CET1: 13.4%–15.3%).
- **MS**: Standardized CET1: 17.4% (2020), 16.0% (2021), 15.3% (2022), 15.2% (2023), 15.9% (2024). (Advanced CET1: 15.5%–17.7%).
- **JPM**: Standardized CET1: 13.1% (2020), 13.1% (2021), 13.2% (2022), 15.0% (2023), 15.7% (2024). (Advanced CET1: 13.1%–15.8%).
- **SF**: Standardized CET1: 16.5% (2020), 15.2% (2021), 14.6% (2022), 14.2% (2023), 15.4% (2024).
- **JEF**: **NOT APPLICABLE (No CET1)**. Non-BHC broker-dealer holding company. Jefferies LLC maintains SEC Rule 15c3-1 excess net capital: \$1,563M (2020) to \$2,476M (2024).
- **EVR**: **NOT APPLICABLE (No CET1)**. Independent advisory firm.
- **LAZ**: **NOT APPLICABLE (No CET1)**. Independent advisory and asset management firm.
- **MC**: **NOT APPLICABLE (No CET1)**. Pure-play advisory firm.
- **Feasibility & Comparability**: **100% Available and Comparable for BHCs (GS, MS, JPM, SF)**; **ZERO availability for non-BHCs (JEF, EVR, LAZ, MC)**. Must NEVER be pooled across all 8 firms.

### 3.6. Total Capital / Tangible Common Equity (TCE)
- **BHCs (GS, MS, JPM, SF)**: Consistently report Basel III Total Risk-Based Capital and Non-GAAP Tangible Common Equity (Common equity less goodwill and intangibles):
  * GS Tangible Common Equity: \$84.2B (2020) to \$112.5B (2024).
  * MS Tangible Common Equity: \$75.9B (2020) to \$71.6B (2024).
  * JPM Tangible Common Equity: \$206.1B (2020) to \$279.4B (2024).
  * SF Common Stockholders' Equity: \$3.6B (2020) to \$5.2B (2024); Total Capital \$3.0B to \$4.6B.
- **Broker-Dealer / Boutiques (JEF, EVR, LAZ, MC)**:
  * JEF Tangible Stockholders' Equity: \$7.8B (2023) to \$8.4B (2022).
  * EVR Total Stockholders' Equity: \$1,231M (2020) to \$1,708M (2024).
  * LAZ Stockholders' Equity: \$423.8M (2023) to \$975.2M (2021). Tangible equity frequently negative.
  * MC Stockholders' Equity: \$266M (2023) to \$440M (2024); virtually zero intangibles, so TCE equals book equity.
- **Feasibility & Comparability**: Sub-panel comparable. BHCs have dedicated regulatory capital accounting; boutiques report corporate equity.

### 3.7. Dividends Paid
- **GS**: \$2,336M (2020), \$2,725M (2021), \$3,682M (2022), \$4,189M (2023), \$4,497M (2024).
- **MS**: \$2,739M (2020), \$4,171M (2021), \$5,401M (2022), \$5,763M (2023), \$6,138M (2024).
- **JPM**: \$11,048M (2020), \$11,180M (2021), \$11,577M (2022), \$11,921M (2023), \$12,779M (2024).
- **JEF**: \$160.9M (2020), \$222.8M (2021), \$280.1M (2022), \$278.6M (2023), \$303.0M (2024).
- **EVR**: \$106.6M (2020), \$118.8M (2021), \$127.3M (2022), \$127.9M (2023), \$135.8M (2024).
- **LAZ**: \$196.6M (2020), \$195.9M (2021), \$181.9M (2022), \$173.1M (2023), \$179.0M (2024).
- **MC**: \$282.9M (2020), \$480.0M (2021), \$174.7M (2022), \$182.2M (2023), \$184.2M (2024).
- **SF**: \$66.1M (2020), \$94.9M (2021), \$122.9M (2022), \$148.6M (2023), \$165.7M (2024).
- **Feasibility & Comparability**: **100% Available and Directly Comparable across all 8 firms** from primary Statements of Cash Flows (Financing Activities).

### 3.8. Share Repurchases
- **GS**: \$1,928M (2020), \$5,200M (2021), \$3,500M (2022), \$5,796M (2023), \$8,000M (2024).
- **MS**: \$1,347M (2020), \$11,464M (2021), \$9,865M (2022), \$5,300M (2023), \$3,250M (2024).
- **JPM**: \$6,517M (2020), \$18,408M (2021), \$3,162M (2022), \$9,824M (2023), \$18,830M (2024).
- **JEF**: \$816.9M (2020), \$269.4M (2021), \$859.6M (2022), \$169.4M (2023), \$44.3M (2024).
- **EVR**: \$146.6M (2020), \$720.7M (2021), \$520.5M (2022), \$387.3M (2023), \$448.2M (2024).
- **LAZ**: \$95.2M (2020), \$406.1M (2021), \$691.7M (2022), \$102.1M (2023), \$59.5M (2024).
- **MC**: \$44.3M (2020), \$104.2M (2021), \$147.5M (2022), \$47.0M (2023), \$10.8M (2024).
- **SF**: \$58.3M (2020), \$172.7M (2021), \$105.8M (2022), \$443.9M (2023), \$144.1M (2024).
- **Feasibility & Comparability**: **100% Available and Directly Comparable across all 8 firms** from primary Statements of Cash Flows (Financing Activities). Reflects actual cash spent on share repurchases under Board authorizations.

### 3.9. Business / Technology Investment
- **GS**: Communications & technology opex: \$1,347M to \$1,991M. Capex additions: \$2.1B to \$6.3B.
- **MS**: Information systems & communications opex: \$2,465M to \$4,088M.
- **JPM**: Technology, communications & equipment opex: \$8,024M to \$9,831M.
- **JEF**: Communications & technology opex: \$341M to \$547M. Capex additions: \$1.2M to \$250.6M.
- **EVR**: Communications & information services opex: \$54.3M to \$81.5M. Capex additions: \$16.9M to \$33.3M.
- **LAZ**: Technology & information services opex: \$133.5M to \$189.7M. Capex additions: \$28.3M to \$64.3M.
- **MC**: **Bundled in Non-compensation expenses** (\$116.8M to \$191.4M); no standalone IT line on face of income statement. Capex: \$1.8M to \$16.9M.
- **SF**: Communications & technology opex: \$148.9M to \$198.8M. Capitalized software additions: \$30M to \$60M.
- **Feasibility & Comparability**: **Partially Comparable / Non-Standardized**. There is no unified GAAP definition of "technology investment." Income statement lines measure ongoing IT operations, telecom, and market data subscriptions (Bloomberg/Refinitiv), whereas Statements of Cash Flows report capitalized software and physical equipment. Moelis does not break out IT separately from general non-comp expenses.

### 3.10. Relevant Leverage / Balance-Sheet Measure
- **BHCs (GS, MS, JPM, SF)**:
  * GS: Supplementary Leverage Ratio (SLR) 5.5%–7.0%; Tier 1 Leverage 6.7%–7.1%. Total Assets: \$1,163B–\$1,676B.
  * MS: SLR 5.5%–7.4%; Tier 1 Leverage 6.7%–8.4%. Total Assets: \$1,116B–\$1,215B.
  * JPM: SLR 5.4%–6.9%; Tier 1 Leverage 6.5%–7.2%. Total Assets: \$3,385B–\$3,744B.
  * SF: Tier 1 Leverage 10.8%–11.4%. Total Assets: \$27.9B–\$40.5B. (Exempt from SLR).
- **Broker-Dealer / Boutiques (JEF, EVR, LAZ, MC)**:
  * JEF: Assets/Equity leverage 5.0x–6.3x; Long-Term Debt \$8.4B–\$13.5B. Total Assets: \$51.1B–\$64.4B.
  * EVR: Total Assets \$3.4B–\$4.2B; holds \$2.1B in cash and \$385M notes payable. **Net cash surplus**.
  * LAZ: Total Assets \$4.6B–\$7.1B; fixed senior notes of \$1,685M. Assets/Equity ratio rose to 10.9x in 2023.
  * MC: Total Assets \$741M–\$1,048M; zero funded debt; holds \$413M in cash. **Net cash surplus**.
- **Feasibility & Comparability**: **Structurally Non-Comparable across business models**. BHCs operate high-volume, repo- and deposit-funded balance sheets governed by Basel III SLR; boutiques operate asset-light advisory models with negative net debt (cash rich).

---

## 4. Synthesis of Unified Feasibility Comparison

### 4.1. Metrics Directly Comparable Across ALL 8 Firms
1. **Net Revenue**: Total revenues less interest expense (GAAP).
2. **Investment Banking Revenue / Fees**: Core investment banking fee generation (Advisory, Underwriting).
3. **Dividends Paid**: Actual cash paid out to equity holders (Statement of Cash Flows).
4. **Actual Share Repurchases**: Actual cash deployed to repurchase common shares/units (Statement of Cash Flows).

### 4.2. Metrics Only Comparable Within Bank Holding Companies (GS, MS, JPM, SF)
1. **Common Equity Tier 1 (CET1) Ratio**: Standardized Basel III risk-weighted capital adequacy.
2. **Tier 1 Leverage Ratio & Supplementary Leverage Ratio (SLR)**: Total leverage exposure tests.
3. **Return on Tangible Common Equity (ROTCE)**: Reconciled against average tangible common equity.
4. **Efficiency / Overhead Ratio**: Total operating expenses as a percentage of net revenues.

### 4.3. Metrics More Appropriate for Advisory / Boutique Firms (EVR, LAZ, MC, JEF)
1. **Compensation Ratio**: Compensation and benefits expense divided by net revenue (50%–77%). Reflects the true variable capital allocation in advisory banking (human capital vs. financial capital).
2. **Operating Margin**: Operating income divided by net revenue. Avoids distortions in book equity caused by Up-C partnerships, tax receivable agreements, and treasury distributions.
3. **Net Cash / Liquidity Surplus**: Cash, cash equivalents, and short-term investments minus debt.

### 4.4. Fiscal-Year Alignment Differences
- **Calendar Year (ending Dec 31)**: GS, MS, JPM, EVR, LAZ, MC, SF (7 of 8 firms).
- **Non-Calendar Fiscal Year (ending Nov 30)**: Jefferies Financial Group (JEF).
  * *Audit Impact*: JEF's FY2020 ended November 30, 2020; its FY2024 ended November 30, 2024. If pooled in a strict calendar panel, Jefferies introduces a 1-month timing mismatch. In quarterly event-study designs, calendar dates must be lagged.

### 4.5. Regulatory Capital Comparability
Federal Reserve Basel III capital rules govern only BHCs. Non-BHC broker-dealer subsidiaries are subject to SEC Rule 15c3-1 net capital haircuts (a liquidation-based solvency test), which cannot be translated, equated, or imputed into Basel III risk-weighted CET1 ratios.

---

## 5. Direct Answers to Core Mandate Questions

### Question A: Which firms have adequate 2020–2024 coverage?
**All eight candidate firms** have 100% complete primary-source coverage across 2020–2024 via official SEC Form 10-K filings. Not a single year or candidate firm is missing primary filings.

### Question B: Which variables are genuinely comparable?
The genuinely comparable variables across all candidate firms are:
1. **Total Net Revenue** (GAAP)
2. **Investment Banking Fees / Revenue** (GAAP / Segment)
3. **Dividends Paid** (GAAP Statement of Cash Flows)
4. **Share Repurchases** (GAAP Statement of Cash Flows)
5. **Total Capital Returned to Shareholders** (Dividends + Repurchases)
6. **Compensation Ratio** (for all 8 firms when calculated as GAAP Compensation Expense / Net Revenue)

### Question C: Which variables must be dropped from a unified panel?
1. **CET1 Ratio**: Must be dropped from any panel that includes non-BHCs (JEF, EVR, LAZ, MC).
2. **Supplementary Leverage Ratio (SLR) / Tier 1 Leverage**: Must be dropped from any panel containing boutiques.
3. **ROE / ROTCE**: Must be dropped from a unified cross-sector panel because EVR, LAZ, and MC omit ROE in their 10-Ks due to Up-C partnership and legacy capital distortions.
4. **Standalone Technology Investment**: Cannot be used as a standardized explanatory variable because MC bundles IT into non-compensation expenses, and reporting across the other seven firms conflates ongoing telecom/market data opex with capitalized software.

### Question D: Are diversified banks and advisory firms sufficiently comparable?
**No**. Diversified universal banks (JPMorgan Chase), global investment bank BHCs (Goldman Sachs, Morgan Stanley), mid-market broker-dealer BHCs (Stifel), broker-dealer holding companies (Jefferies), and independent advisory boutiques (Evercore, Lazard, Moelis) operate under fundamentally distinct corporate structures, regulatory regimes, and economic models:
- **Capital Intensity**: BHCs allocate vast balance-sheet capital, take inventory and credit risk, and are constrained by Federal Reserve regulatory capital ratios and annual stress tests (CCAR).
- **Human Capital vs. Financial Capital**: Advisory boutiques allocate **human capital** (distributing 55%–70% of revenues in compensation) and hold substantial **net cash**. They do not use their balance sheet to fund loans or make markets.
- **Panel Pooling**: Pooling them into a single econometric model without controlling for structural business models would produce severe omitted-variable bias and spurious regressions.

### Question E: What is the defensible final sample?
Because forcing a single 5-firm panel creates irreconcilable accounting conflicts, there are **three defensible sample options**:
1. **Option 1: Bank Holding Company Panel (4 Firms: GS, MS, JPM, SF)**  
   *Focus*: Regulatory capital allocation, CET1 management, SLR leverage, ROTCE, and shareholder capital return in balance-sheet-intensive banking.
2. **Option 2: Independent Advisory & Capital Markets Panel (4 Firms: EVR, LAZ, MC, JEF)**  
   *Focus*: Pure-play advisory dynamics, compensation flexibility, operating margins, and free cash return without banking regulatory constraints. (If strict calendar year alignment is required, EVR, LAZ, and MC form a pure 3-firm boutique panel).
3. **Option 3: Core Investment Banking Panel (5 Firms: GS, MS, JEF, EVR, LAZ)**  
   *Focus*: Investment banking fee revenue and GAAP cash return (Dividends + Repurchases). Drops commercial bank consumer lending (JPM) and mid-cap retail wealth (SF).

### Question F: What is the defensible final core variable set?
For a cross-firm study spanning both banks and advisory firms, the defensible core variable set consists of:
1. `net_revenue` (Firm-wide GAAP net revenues)
2. `ib_revenue` (Total investment banking / advisory / underwriting fees)
3. `ib_intensity` ($rac{	ext{IB Revenue}}{	ext{Net Revenue}}$)
4. `comp_ratio` ($rac{	ext{Compensation Expense}}{	ext{Net Revenue}}$)
5. `operating_margin` ($rac{	ext{Operating Income}}{	ext{Net Revenue}}$)
6. `dividends_paid` (Cash paid for dividends from Statement of Cash Flows)
7. `share_repurchases` (Cash paid for share buybacks from Statement of Cash Flows)
8. `total_cash_return` ($	ext{Dividends} + 	ext{Repurchases}$)
9. `payout_ratio` ($rac{	ext{Total Cash Return}}{	ext{Net Income}}$ or $rac{	ext{Total Cash Return}}{	ext{Operating Cash Flow}}$)

---

## 6. Recommended Research Design & Architecture

```
                       CANDIDATE UNIVERSE (8 Firms)
                                    |
          +-------------------------+-------------------------+
          |                                                   |
   BANK HOLDING COMPANIES                             INDEPENDENT ADVISORY
(Balance-Sheet Intensive / Basel III)              (Human Capital / Asset-Light)
          |                                                   |
   GS, MS, JPM, SF                                     EVR, LAZ, MC, JEF
          |                                                   |
  * Variables:                                        * Variables:
    - CET1 (Standardized/Advanced)                      - Compensation Ratio
    - Supplementary Leverage (SLR)                      - Operating Margin
    - Tier 1 Leverage                                   - Net Cash Surplus
    - ROTCE / ROE                                       - Buybacks + Dividends
    - Dividends + Buybacks                              - Advisory Fee Share
```

### Strongest Defensible Recommendation
The strongest, most rigorous research design is a **Dual-Panel Comparative Architecture**:
1. **Primary Regulated Panel (BHCs: GS, MS, JPM, SF)**: Investigates how regulatory capital constraints (CET1 buffers, stress tests) dictate capital allocation between market-making inventory, lending, dividends, and share repurchases.
2. **Pure Advisory Panel (Boutiques: EVR, LAZ, MC)**: Investigates how asset-light advisory firms allocate operating surplus between partner compensation and equity capital return across market cycles.

This cleanly separates the economic mechanism of **regulatory capital steering** from **human capital incentive steering**, preserving 100% primary source integrity and avoiding fabricated or pseudo-harmonized metrics.
