# Phase 4 Analysis Report: Descriptive and Longitudinal Analysis of Strategic Capital Allocation in Investment Banking (2020–2024)

**Author**: 12th-Grade Independent Student Research Project  
**Project Title**: Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024  
**Date**: September 2026  
**Target Period**: Fiscal Years 2020, 2021, 2022, 2023, and 2024  
**Status**: Phase 4 Complete (Descriptive, Longitudinal, and Exploratory Lagged Analysis)  

---

## 1. Purpose of the Study

The purpose of this research project is to examine how major investment banking and financial advisory firms allocated capital across the five-year period from 2020 through 2024, and how those capital decisions were associated with subsequent business performance.

In corporate finance, capital allocation refers to how executive leadership distributes financial resources. When an investment bank earns revenues, it faces choices regarding how to divide that cash:
1. Distributing capital back to shareholders through regular cash dividends.
2. Repurchasing common stock in the open market to return excess capital or offset equity dilution.
3. Retaining capital on the balance sheet to maintain regulatory capital reserves (such as Common Equity Tier 1 capital in bank holding companies) or corporate liquidity cushions.
4. Reinvesting in personnel through annual incentive compensation pools and technology infrastructure.

The core research question guiding this investigation is:
> *"How do major investment-banking firms allocate capital between business investment, capital retention, and shareholder distributions, and how are these patterns associated with subsequent business performance?"*

To examine this question objectively, I analyzed the financial reports of eight leading Wall Street firms over a five-year period characterized by extreme macroeconomic shifts: the initial emergency response and monetary stimulus of the 2020 COVID-19 pandemic, the record investment-banking underwriting and advisory boom of 2021, the rapid Federal Reserve interest-rate hiking cycle of 2022, the advisory deal trough and regional banking stresses of 2023, and the cyclical recovery of 2024.

This study is an observational analysis. Because corporate capital allocation decisions occur in complex, dynamic market environments, this study does not attempt to establish causal proof. The focus throughout this report is on identifying observable patterns, calculating descriptive changes over time, comparing differences across distinct business models, and evaluating exploratory one-year lagged relationships.

---

## 2. Dataset and Source Provenance

The empirical dataset examined in this report was collected directly from first-party regulatory filings with the U.S. Securities and Exchange Commission (SEC). Rather than utilizing aggregated secondary databases or third-party web platforms, every observation was extracted from audited annual Form 10-K filings and official SEC XBRL company facts.

Collected observations were linked to SEC filings through the project provenance map (`PHASE3_PROVENANCE_MAP.csv`), which records the specific 20-digit accession number, financial statement, disclosure footnote, reported accounting terminology, and EDGAR URL for every data point.

The dataset encompasses:
- **8 Candidate and Sensitivity Firms**: Organised into two primary panels and one sensitivity group.
- **5 Fiscal Years**: 2020, 2021, 2022, 2023, and 2024 strictly (with zero post-2024 observations).
- **540 Audited Raw Observations**: Covering revenues, underwriting fees, cash dividends, share repurchases, regulatory capital ratios, compensation expenses, and balance-sheet liquidity.
- **70 Derived Observations**: Calculated through explicit mathematical formulas (such as total cash returned to shareholders, boutique net cash cushions, and operating margins).
- **40 Primary Form 10-K Filings**: Spanning 2020 through 2024 across all eight firms.

### Panel Architecture
Because investment banks operate under fundamentally different business models and regulatory regimes, pooling all firms into a single uniform panel would create severe accounting distortions. The analysis therefore adheres to the two-panel architecture locked in Phase 1:

1. **Panel A: Bank Holding Companies (4 Firms)**:
   - *The Goldman Sachs Group, Inc. (`GS`)*: Global investment banking, trading, and asset management (Category I G-SIB).
   - *Morgan Stanley (`MS`)*: Global investment banking, institutional trading, and wealth management (Category I G-SIB).
   - *JPMorgan Chase & Co. (`JPM`)*: Universal banking giant; firm-wide capital and Commercial & Investment Bank (CIB) operations (Category I G-SIB).
   - *Stifel Financial Corp. (`SF`)*: Financial holding company with strong wealth management and middle-market investment banking (Category IV regional bank).
   - *Core Analytical Metrics*: Net revenue, investment banking revenue, return on common equity (ROE), return on tangible common equity (ROTCE), efficiency/overhead ratio, standardized Common Equity Tier 1 (CET1) ratio, Tier 1 leverage ratio, cash dividends paid, and common share repurchases.

2. **Panel B: Independent Advisory Boutiques (3 Firms)**:
   - *Evercore Inc. (`EVR`)*: Premier independent advisory boutique.
   - *Lazard, Inc. (`LAZ`)*: International financial advisory and asset management firm.
   - *Moelis & Company (`MC`)*: Pure-play independent global advisory firm.
   - *Core Analytical Metrics*: Net revenue, advisory/underwriting fees, compensation and benefits expense, compensation expense ratio, operating income, operating margin, cash dividends/partnership distributions paid, and share repurchases.

3. **Context / Sensitivity Group (1 Firm)**:
   - *Jefferies Financial Group Inc. (`JEF`)*: Full-service broker-dealer holding company. Jefferies is isolated from Panel A and Panel B pooling because its fiscal year ends on November 30 (one month ahead of calendar year-end firms) and it is regulated under SEC broker-dealer net capital rules (SEC Rule 15c3-1) rather than Federal Reserve bank holding company Basel III regulations.

---

## 3. Descriptive Findings Across the Full Cycle

Across the entire five-year period, the collected data illustrates the cyclicality of investment banking revenues and the varied ways firms managed their payouts.

```
+----------------------------------------------------------------------------------------------------+
|                                    FIVE-YEAR REVENUE SUMMARY (USD Millions)                        |
+--------+-----------------+----------------------------------+--------------------------------------+
| Ticker | Panel Group     | 5-Year Mean Net Revenue          | 5-Year Mean Investment Banking Fees  |
+--------+-----------------+----------------------------------+--------------------------------------+
| GS     | Panel A (BHC)   | $50,205.4M                       | $9,122.6M                            |
| MS     | Panel A (BHC)   | $55,524.2M                       | $7,152.2M                            |
| JPM    | Panel A (BHC)   | $139,629.0M                      | $8,962.4M                            |
| SF     | Panel A (BHC)   | $4,860.9M                        | $1,081.0M                            |
+--------+-----------------+----------------------------------+--------------------------------------+
| EVR    | Panel B (Bout.) | $2,762.1M                        | $2,721.7M                            |
| LAZ    | Panel B (Bout.) | $2,897.8M                        | $1,624.2M                            |
| MC     | Panel B (Bout.) | $1,103.7M                        | $1,103.7M                            |
+--------+-----------------+----------------------------------+--------------------------------------+
| JEF    | Sensitivity     | $8,186.3M                        | $2,998.3M                            |
+--------+-----------------+----------------------------------+--------------------------------------+
```

### The 2020–2024 Market Cycle Stages

The five-year study period unfolded through four distinct operating phases:

1. **2020 (Pandemic Shock and Initial Response)**:
   Net revenues remained resilient due to strong market liquidity and initial debt refinancing. However, shareholder distributions were constrained. In Panel A, total cash returned averaged $6,922.3M per firm, with Goldman Sachs returning $4,264.0M (9.57% of net revenue) and Morgan Stanley returning $4,086.0M (8.48% of net revenue). Firms built balance-sheet cash and maintained conservative payout ratios amid economic uncertainty.

2. **2021 (The Industry Peak)**:
   The year 2021 was an extraordinary boom year for investment banking across all eight firms. Advisory fees and equity underwriting surged to historic highs. Goldman Sachs earned $14,877.0M in investment banking revenue (a 57.9% increase over 2020), while JPMorgan earned $13,215.0M. Independent boutiques experienced comparable growth: Evercore generated $3,288.4M in advisory fees (+46.1%), and Moelis generated $1,540.6M (+63.3%). 
   Operating margins expanded sharply in 2021 (Evercore reached 27.61%, Moelis reached 27.16%, and Lazard reached 22.59%). In response to this earnings expansion, firms increased share repurchases: Morgan Stanley repurchased $11,464.0M of common stock (up from $1,347.0M in 2020), and JPMorgan repurchased $18,408.0M (up from $6,517.0M in 2020).

3. **2022–2023 (The Cyclical Contraction and Deal Trough)**:
   Beginning in early 2022, the Federal Reserve initiated an aggressive monetary tightening cycle, raising the federal funds target rate by more than 500 basis points. Global M&A completions and debt/equity underwriting declined sharply. Goldman Sachs' investment banking revenue dropped to $7,360.0M in 2022 and $6,218.0M in 2023 (a 58.2% decline from its 2021 peak). Morgan Stanley's investment banking fees fell to $4,635.0M in 2023.
   Among advisory boutiques, revenues contracted while personnel costs remained relatively inflexible. Compensation ratios rose from ~60% in 2021 to 66.0% at Evercore, 70.0% at Moelis, and 71.6% at Lazard in 2023. Operating margins contracted to 14.5% at Evercore, 7.4% at Moelis, and 5.1% at Lazard. 

4. **2024 (The Cyclical Recovery)**:
   In 2024, announced transactions and underwriting activity began to normalize. Investment banking revenue rebounded across all eight firms: Goldman Sachs reached $7,738.0M (+24.4% over 2023), Morgan Stanley reached $6,664.0M (+43.8%), Evercore reached $2,933.2M (+22.8%), and Moelis reached $1,194.5M (+39.8%). Operating margins in Panel B expanded back toward long-term averages.

---

## 4. Changes from 2020 to 2024

To assess how capital allocation evolved over the full five-year arc, I calculated the net change between the baseline year (2020) and the final year (2024) for each firm.

```
+----------------------------------------------------------------------------------------------------+
|                                    2020 TO 2024 WITHIN-FIRM CHANGES                                |
+--------+--------------------+---------------------+--------------------+---------------------------+
| Ticker | Net Revenue Change | IB Revenue Change   | Dividends Change   | Share Repurchases Change  |
+--------+--------------------+---------------------+--------------------+---------------------------+
| GS     | +$8,950.0M (+20.1%)| -$1,682.0M (-17.9%) | +$2,161.0M (+92.5%)| +$6,072.0M (+314.9%)      |
| MS     | +$13,617.0M(+28.3%)| -$2,277.0M (-25.5%) | +$3,399.0M(+124.1%)| +$1,903.0M (+141.3%)      |
| JPM    | +$50,611.0M(+42.3%)| -$364.0M   (-3.8%)  | +$2,093.0M (+16.5%)| +$12,313.0M(+188.9%)      |
| SF     | +$2,133.9M (+55.9%)| -$55.4M    (-5.0%)  | +$153.5M  (+208.0%)| +$85.8M    (+147.2%)      |
| EVR    | +$711.1M   (+31.1%)| +$682.5M   (+30.3%) | +$39.4M   (+37.0%) | +$291.4M   (+198.8%)      |
| LAZ    | +$493.1M   (+18.6%)| +$341.9M   (+24.3%) | -$16.5M   (-8.2%)  | -$36.8M    (-40.4%)       |
| MC     | +$251.2M   (+26.6%)| +$251.2M   (+26.6%) | -$0.4M    (-0.2%)  | -$131.8M   (-84.5%)       |
| JEF    | +$3,634.7M (+52.8%)| +$592.2M   (+21.1%) | +$100.6M  (+60.7%) | -$731.1M   (-90.0%)       |
+--------+--------------------+---------------------+--------------------+---------------------------+
```

### Key Within-Firm Observations:
1. **Top-Line Net Revenue Growth**: All eight firms recorded higher net revenues in 2024 than in 2020. Among large bank holding companies, net revenue expansion was supported by higher net interest income during the Federal Reserve rate hiking cycle (especially at JPMorgan, whose net revenue expanded by +$50,611.0M or +42.3%, also incorporating the First Republic acquisition in 2023).
2. **Investment Banking Fee Divergence**: In the large diversified bank holding companies (GS, MS, JPM, SF), investment banking revenue in 2024 was lower than in 2020. This reflects the unusually elevated debt underwriting levels present in 2020 during emergency pandemic corporate liquidity raising. Conversely, the pure-play and advisory boutiques (EVR, LAZ, MC) recorded higher fee revenues in 2024 than in 2020, as M&A advisory advisory fees rebounded.
3. **Dividend Asymmetry vs. Repurchase Volatility**: Across the entire universe, cash dividends paid showed continuous upward or stable trajectories, whereas share repurchases fluctuated widely from year to year. In Panel A, annual dividend payouts expanded by +92.5% at Goldman Sachs, +124.1% at Morgan Stanley, +16.5% at JPMorgan, and +208.0% at Stifel. Share repurchases expanded during high-earnings years (2021 and 2024) but were curtailed during contraction years.

---

## 5. Panel A — Bank Holding Company Results

Panel A examines the four bank holding companies: Goldman Sachs, Morgan Stanley, JPMorgan Chase, and Stifel Financial.

### Regulatory Capital and Balance Sheet Structure
Under the Federal Reserve's Basel III framework, bank holding companies report standardized risk-weighted capital ratios. The Standardized Common Equity Tier 1 (CET1) ratio serves as the primary benchmark:

- **Goldman Sachs**: Standardized CET1 was 14.7% in 2020, dipped to 14.2% in 2021 as balance-sheet assets expanded, rose to 15.0% in 2022, and closed 2024 at 14.8%.
- **Morgan Stanley**: Reported Standardized CET1 of 17.4% in 2020 following the E*TRADE acquisition, adjusting to 15.2% by 2024.
- **JPMorgan Chase**: Rose steadily from 13.1% in 2020 to 15.3% in 2024, building capital reserves through retained earnings.
- **Stifel Financial**: Maintained a consistent CET1 ratio around 11.2%–11.7% across the entire five-year window (averaging 11.46%).

### Supplementary Leverage Ratio (SLR) Dynamics
The Supplementary Leverage Ratio measures Tier 1 capital relative to total leverage exposure (including off-balance-sheet derivatives and commitments). 
- In 2020, the Federal Reserve provided temporary regulatory relief allowing large banks to exclude U.S. Treasuries and deposits at Federal Reserve banks from leverage calculations. Consequently, 2020 SLR ratios were temporarily elevated: Goldman Sachs reported 7.0%, Morgan Stanley 7.4%, and JPMorgan 6.9%.
- Following the expiration of this temporary relief on March 31, 2021, reported SLR ratios adjusted downward: by 2023, Goldman Sachs reported 5.4%, Morgan Stanley 5.2%, and JPMorgan 5.3%.
- Stifel Financial is classified as a Category IV banking organization under Federal Reserve tailoring rules and is legally exempt from calculating or publishing an SLR ratio. This observation was appropriately designated `NOT_APPLICABLE` and excluded from numeric computations.

### Operating Efficiency and Return on Equity
Operating performance in Panel A tracked market activity:
- **Return on Common Equity (ROE)**: Peaked in 2021 across all four institutions (Goldman Sachs reached 23.0%, JPMorgan reached 19.0%, Stifel reached 20.3%, and Morgan Stanley reached 15.0%). In 2023, ROE compressed to 7.5% at Goldman Sachs, 9.4% at Morgan Stanley, and 11.4% at Stifel, before recovering in 2024 (Goldman Sachs 11.0%, Morgan Stanley 11.8%, JPMorgan 17.0%, and Stifel 12.5%).
- **Efficiency Ratio (Overhead Ratio)**: Exhibits an inverse relationship with profitability. Lower percentages reflect lower operating costs relative to revenues. During the 2021 peak, Goldman Sachs recorded an efficiency ratio of 53.8%. In the 2023 trough, as advisory revenues contracted while fixed operational and compensation expenses remained, the ratio rose to 74.7% at Goldman Sachs, 77.0% at Morgan Stanley, and 82.2% at Stifel.

---

## 6. Panel B — Advisory Boutique Results

Panel B analyzes the independent advisory boutiques: Evercore, Lazard, and Moelis & Company.

### Asset-Light Operating Models
Unlike bank holding companies, advisory boutiques do not maintain deposit-taking banking franchises or multi-hundred-billion-dollar trading balance sheets. They operate asset-light advisory models where personnel and intellectual capital are the primary revenue generators.

- **Compensation Expense Ratios**: The compensation expense ratio (compensation expense divided by net revenue) is a key reported metric for advisory boutiques. Across 2020–2024:
  - At Evercore, the compensation ratio averaged 63.46% (ranging from a low of 60.1% in 2022 to a high of 66.0% in 2023 and 2024).
  - At Lazard, the ratio averaged 64.02% (ranging from 61.1% in 2021–2022 to a peak of 71.6% in 2023).
  - At Moelis, the ratio averaged 65.40% (ranging from 63.0% in 2020 to 70.0% in 2023).
- **Movement During Lower-Revenue Years**: In 2023, when net revenues declined by -26.1% at Evercore and -44.5% at Moelis relative to their 2021 peaks, compensation ratios rose to cycle highs (66.0% to 71.6%), as total compensation expense declined by a smaller percentage than net revenue.

### Operating Margins and Net Cash Cushions
Operating margins in Panel B moved in direct alignment with advisory deal volume:
- During the 2021 boom, operating margins reached 27.61% at Evercore, 27.16% at Moelis, and 22.59% at Lazard.
- During the 2023 contraction, operating margins compressed to 15.00% at Evercore, 7.41% at Moelis, and 5.12% at Lazard.
- **Liquidity and Funded Debt**: Evercore and Moelis maintained zero funded long-term debt across the entire five-year study period, holding positive net cash cushions that averaged $611.5M at Evercore and $299.2M at Moelis. In contrast, Lazard carried senior notes averaging $1,684.9M against cash balances of $1,326.3M, resulting in a net debt position averaging -$358.7M.

---

## 7. Common-Core Descriptive Comparison

The Common GAAP Core encompasses the five variables that are consistently reported under U.S. GAAP across all eight firms: Net Revenue, Investment Banking Revenue, Cash Dividends Paid, Share Repurchases, and Total Cash Returned.

```
+----------------------------------------------------------------------------------------------------+
|                               COMMON CORE 5-YEAR TOTAL CASH RETURNED                               |
+--------+------------------+---------------------+---------------------+----------------------------+
| Ticker | 5-Year Net Rev.  | 5-Year Dividends    | 5-Year Repurchases  | Total Cash Returned ($ / %)|
+--------+------------------+---------------------+---------------------+----------------------------+
| GS     | $251,027.0M      | $17,429.0M          | $24,424.0M          | $41,853.0M (16.7%)         |
| MS     | $277,621.0M      | $24,212.0M          | $31,226.0M          | $55,438.0M (20.0%)         |
| JPM    | $698,145.0M      | $67,356.0M          | $56,741.0M          | $124,097.0M (17.8%)        |
| SF     | $24,304.7M       | $774.3M             | $924.9M             | $1,699.2M  (7.0%)          |
| EVR    | $13,810.4M       | $624.5M             | $2,215.0M           | $2,839.5M  (20.6%)         |
| LAZ    | $14,488.9M       | $986.7M             | $1,294.4M           | $2,281.1M  (15.7%)         |
| MC     | $5,518.4M        | $1,168.9M           | $488.8M             | $1,657.7M  (30.0%)         |
| JEF    | $40,931.7M       | $1,276.7M           | $2,028.3M           | $3,305.0M  (8.1%)          |
+--------+------------------+---------------------+---------------------+----------------------------+
```

### Observations from the Common Core:
1. **Aggregate Volume**: Over the five-year period, the eight firms returned an aggregate of **$233,169.5M** in cash to shareholders ($113,828.1M in cash dividends and $119,341.4M in share repurchases).
2. **Payout Proportions Across Models**: As a percentage of five-year net revenue, total cash returned was highest at Moelis & Company (30.0%), followed by Evercore (20.6%) and Morgan Stanley (20.0%). Universal and commercial-focused banks returned between 7.0% (Stifel) and 17.8% (JPMorgan).
3. **Dividend Stability vs. Repurchase Flexibility**: Across all firms, cash dividends functioned as a recurring baseline payout, while share repurchases functioned as a shock absorber. In 2021, share repurchases accounted for 73.3% of total cash returned at Morgan Stanley and 85.9% at Evercore. During the 2022–2023 downturn, repurchases were curtailed while dividends continued to be paid.

---

## 8. Exploratory Lagged Associations ($t 	o t+1$)

To evaluate whether capital allocation decisions in one year were associated with operating performance in the subsequent year, I analyzed one-year lagged relationships ($t 	o t+1$).

Because the dataset covers five fiscal years (2020–2024), each firm contributes a maximum of four annual transitions:
- $2020 	o 2021$
- $2021 	o 2022$
- $2022 	o 2023$
- $2023 	o 2024$

This yields a maximum sample size of $N=16$ for Panel A (4 firms $	imes$ 4 transitions) and $N=12$ for Panel B (3 firms $	imes$ 4 transitions). Both Pearson correlation ($r$) and Spearman rank correlation ($ho$) were calculated.

```
+----------------------------------------------------------------------------------------------------+
|                         EXPLORATORY LAGGED ASSOCIATION MATRIX (t -> t+1)                           |
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
| Panel   | Predictor ($t$)        | Outcome ($t+1$)   | N  | Pearson r | p-value | Spearm. ρ | p-val|
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
| Panel A | Share Repurchases      | ROE               | 16 | -0.049    | 0.858   | -0.035    | 0.897|
| Panel A | Share Repurchases      | Efficiency Ratio  | 16 | +0.030    | 0.914   | +0.068    | 0.803|
| Panel A | Cash Dividends Paid    | ROE               | 16 | +0.266    | 0.319   | +0.159    | 0.557|
| Panel A | Cash Dividends Paid    | Efficiency Ratio  | 16 | -0.483    | 0.058   | -0.218    | 0.418|
| Panel A | Standardized CET1      | ROE               | 16 | +0.174    | 0.520   | +0.162    | 0.549|
| Panel A | Standardized CET1      | Efficiency Ratio  | 16 | +0.204    | 0.449   | +0.359    | 0.172|
| Panel A | IB Revenue             | ROE               | 16 | +0.089    | 0.742   | +0.141    | 0.602|
| Panel A | Total Cash Returned    | ROE               | 16 | +0.119    | 0.662   | +0.138    | 0.610|
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
| Panel B | Share Repurchases      | Operating Margin  | 12 | -0.403    | 0.194   | -0.385    | 0.217|
| Panel B | Total Cash Returned    | Operating Margin  | 12 | -0.371    | 0.234   | -0.224    | 0.484|
| Panel B | Compensation Ratio     | Operating Margin  | 12 | -0.036    | 0.912   | -0.102    | 0.753|
| Panel B | Compensation Ratio     | Operating Income  | 12 | -0.152    | 0.637   | -0.186    | 0.564|
| Panel B | IB Revenue             | Operating Margin  | 12 | +0.114    | 0.724   | +0.028    | 0.931|
| Panel B | IB Revenue             | Operating Income  | 12 | +0.470    | 0.123   | +0.503    | 0.095|
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
```

### Detailed Findings from the Lagged Analysis:
1. **Absence of Linear Payout-to-ROE Relationship in Panel A**:
   In Panel A, the relationship between lagged share repurchases in year $t$ and next-year ROE ($t+1$) was close to zero ($r = -0.049$, $p = 0.858$; $ho = -0.035$, $p = 0.897$). Similarly, lagged total cash returned showed a weak positive association with next-year ROE ($r = +0.119$, $p = 0.662$). This indicates that simply returning capital in one year was not systematically associated with higher profitability in the following year.
2. **Dividends and Efficiency in Panel A**:
   Lagged dividends paid showed a moderate negative correlation with next-year efficiency ratio ($r = -0.483$, $p = 0.058$; $ho = -0.218$, $p = 0.418$). Because lower efficiency ratios represent lower expenses relative to revenue, this negative correlation indicates that higher dividend payments coincided with lower subsequent expense ratios. However, the divergence between Pearson $r$ (-0.483) and Spearman $ho$ (-0.218) highlights the influence of firm size (JPMorgan's large dividends).
3. **Negative Payout-to-Margin Association in Panel B**:
   In Panel B, lagged share repurchases showed a negative association with next-year operating margin ($r = -0.403$, $p = 0.194$; $ho = -0.385$, $p = 0.217$). This pattern occurred because peak share buybacks took place in 2021 at the height of the market, which was immediately followed by the 2022 cyclical industry contraction when operating margins compressed.
4. **IB Revenue Persistence in Panel B**:
   Lagged investment banking revenue in year $t$ was positively associated with next-year operating income ($t+1$) among boutiques ($r = +0.470$, $p = 0.123$; $ho = +0.503$, $p = 0.095$). This was one of the more consistent exploratory relationships, reflecting some continuity in advisory fee momentum across consecutive years.

---

## 9. What the Data Suggests

When evaluated with appropriate academic caution, the descriptive and longitudinal patterns indicate several structural characteristics of capital allocation across 2020–2024:

1. **Observed Dividend Stability and Repurchase Variation**:
   Across both bank holding companies and advisory boutiques, regular cash dividends followed a steady or increasing path, while share repurchases exhibited wide year-to-year variation across all firms.
2. **Advisory Boutique Compensation and Operating Margins**:
   Compensation ratios increased for several advisory firms during lower-revenue years, while operating margins also declined. Specifically, during the 2022–2023 revenue downturn, boutique compensation ratios reached 66% to 71%, coinciding with lower operating margins.
3. **Bank Holding Company Capital Ratios**:
   Reported standardized CET1 ratios for the BHC firms ranged from 13.1% to 17.4% during 2020–2024.
4. **Industry-Wide Revenue and Margin Fluctuations**:
   The broad movement of revenues, margins, and returns across all eight firms moved in similar directions over 2020–2024 (elevated levels in 2021, lower levels in 2022–2023, and recovery in 2024).

---

## 10. What the Data Cannot Establish

It is critical to distinguish between observable patterns and unproven assertions. The dataset **cannot** establish the following:

1. **No Evidence of Causality**: The data cannot establish a causal link showing that higher share repurchases led to lower future operating margins, or that building CET1 capital produced changes in bank efficiency. Capital allocation decisions and operating results were both observed within broader macroeconomic and market conditions.
2. **No Evidence of Management Motives**: The financial statements record the dollars spent on dividends, repurchases, and compensation, but they do not reveal executive rationale. The data cannot establish why executive leadership chose specific payout levels or whether compensation decisions targeted specific retention goals.
3. **No Definitive Long-Term Performance Impacts**: Because this study examined a five-year window with one-year lags ($t 	o t+1$), it cannot determine whether capital retention or payout decisions produced advantages over longer multi-decade horizons.
4. **No Superiority of Business Models**: The data shows that boutiques recorded higher operating margins than banks during peak market years, but also experienced sharper margin compression during downturns. The data does not establish that one model is inherently superior or more resilient.

---

## 11. Limitations of the Research

This study was conducted within explicit methodological and practical boundaries:

1. **Small Sample Size ($N=16$ for Panel A, $N=12$ for Panel B)**:
   Because the dataset is limited to five fiscal years across eight firms, the number of annual transitions is necessarily small. With 12 to 16 observations, correlation coefficients and $p$-values must be treated as purely exploratory indicators rather than conclusive statistical tests.
2. **Extreme Cyclical Volatility**:
   The 2020–2024 period was marked by historic events (the COVID-19 pandemic, zero interest rate policy, sudden 525-basis-point rate hikes, and regional bank failures). This macro volatility makes it difficult to separate routine capital allocation effects from macro-driven shocks.
3. **Reporting and Regulatory Disparities**:
   Although data was audited against official SEC filings, institutional differences remain:
   - Stifel is legally exempt from SLR reporting under Federal Reserve Category IV rules.
   - Moelis bundles technology expenses into general operating expenses.
   - Jefferies operates on a November 30 fiscal year under broker-dealer net capital rules, preventing direct pooling.
4. **Observational Design**:
   The study does not utilize natural experiments, instrumental variables, or randomized controls. All findings are strictly correlational.

---

## 12. Summary and Conclusion

This research project investigated how eight major investment banking and advisory firms allocated capital between business investment, regulatory capital reserves, and shareholder distributions over the five-year period from 2020 through 2024.

### Key Empirical Findings

- **Capital Returns Totaled $233.2 Billion**: Over the five-year period, the eight firms returned an aggregate of $113.8B in cash dividends and $119.3B in share repurchases.
- **Observed Dividend Stability and Repurchase Variation**: Across all firms, annual cash dividends remained stable or increased across the five-year period (+92.5% at Goldman Sachs, +124.1% at Morgan Stanley), whereas share repurchases exhibited wide year-to-year variation.
- **Advisory Boutique Compensation and Operating Margins**: Compensation ratios increased for several advisory firms during lower-revenue years, while operating margins also declined. Specifically, boutique compensation ratios ranged from ~61% during the 2021 peak to 66%–71% in 2023, while operating margins contracted before recovering in 2024.
- **Bank Holding Company Capital Ratios**: Reported standardized CET1 ratios for the BHC firms ranged from 13.1% to 17.4% during 2020–2024.
- **Exploratory Lagged Associations**: The relationship between prior-year share repurchases and next-year ROE was close to zero in this small exploratory sample ($r = -0.049$, $p = 0.858$; $\rho = -0.035$, $p = 0.897$, $N=16$).

Dataset ready for Phase 4 review.
