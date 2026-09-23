# Phase 5 Discussion: Strategic Capital Allocation in Investment Banking (2020–2024)

**Project Title**: Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024  
**Researcher**: Ege Can (12th-Grade Independent Student Researcher)  
**Date**: September 2026  
**Status**: Author-Led Discussion & Interpretation  

---

## Introduction and Overview

In this independent research project, I examined how eight major investment-banking and financial advisory firms allocated capital between 2020 and 2024, and how those capital-allocation choices related to subsequent financial performance.

To investigate this question with clear comparability, the study divided the candidate universe into two primary panels alongside one sensitivity firm:
- **Panel A (Bank Holding Companies)**: Goldman Sachs, Morgan Stanley, JPMorgan Chase, and Stifel Financial.
- **Panel B (Independent Advisory Boutiques)**: Evercore, Lazard, and Moelis & Company.
- **Sensitivity Comparison**: Jefferies Financial Group, evaluated separately due to its November 30 fiscal year-end and broker-dealer regulatory framework.

Across the five-year period, the collected data revealed several prominent empirical observations:
1. **Large Aggregate Shareholder Distributions**: The eight firms returned an aggregate of **$233.2 billion** to equity holders ($113.8 billion through cash dividends and $119.3 billion through common share repurchases).
2. **Payout Stability versus Fluctuation**: Across all firms, annual cash dividends followed a steady or increasing path (+92.5% at Goldman Sachs, +124.1% at Morgan Stanley, +16.5% at JPMorgan Chase, and +208.0% at Stifel). In contrast, common share repurchases showed large annual swings, expanding during the 2021 market high and contracting during the 2022–2023 market slowdown.
3. **Net Revenue Growth**: All eight firms reported higher total net revenues in 2024 than in 2020. However, the path differed substantially across firm types: diversified banks experienced revenue support from net interest income during the Federal Reserve rate-hiking cycle, while pure advisory boutiques experienced sharper fluctuations tied to corporate advisory cycles.
4. **Bank Holding Company Capital Bounds**: Reported Standardized Common Equity Tier 1 (CET1) capital ratios for the bank holding companies ranged between 13.1% and 17.4% across all five years, remaining consistently above regulatory minimums.
5. **Advisory Boutique Compensation and Margins**: Advisory boutique compensation ratios increased from 60.1%–64.0% during the 2021 revenue peak to 66.0%–71.6% during the 2023 revenue downturn, while operating margins contracted from 20%–28% in 2021 to 5.1%–15.0% in 2023 before rebounding in 2024.

The sections that follow present my interpretation of what these findings suggest, how different business models shape financial variables, and what limitations must be kept in mind.

---

## 5.1 Different Patterns Across the Two Panels

One of the most surprising observations in this study was that the two panels did not show the same relationships between financial variables, even when similar capital-allocation measures were examined.

When analyzing one-year lagged relationships ($t \to t+1$) across the four annual transitions ($2020 \to 2021$, $2021 \to 2022$, $2022 \to 2023$, and $2023 \to 2024$), the data revealed distinctly different association patterns between the bank holding companies in Panel A and the advisory boutiques in Panel B:

```
+----------------------------------------------------------------------------------------------------+
|                         EXPLORATORY LAGGED CORRELATIONS (t -> t+1)                                 |
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
| Panel   | Predictor ($t$)        | Outcome ($t+1$)   | N  | Pearson r | p-value | Spearm. ρ | p-val|
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
| Panel A | Share Repurchases      | ROE               | 16 | -0.049    | 0.858   | -0.035    | 0.897|
| Panel A | Cash Dividends Paid    | ROE               | 16 | +0.266    | 0.319   | +0.159    | 0.557|
| Panel A | Cash Dividends Paid    | Efficiency Ratio  | 16 | -0.483    | 0.058   | -0.218    | 0.418|
| Panel A | Standardized CET1      | ROE               | 16 | +0.174    | 0.520   | +0.162    | 0.549|
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
| Panel B | Share Repurchases      | Operating Margin  | 12 | -0.403    | 0.194   | -0.385    | 0.217|
| Panel B | Total Cash Returned    | Operating Margin  | 12 | -0.371    | 0.234   | -0.224    | 0.484|
| Panel B | Compensation Ratio     | Operating Margin  | 12 | -0.036    | 0.912   | -0.102    | 0.753|
| Panel B | IB Revenue             | Operating Income  | 12 | +0.470    | 0.123   | +0.503    | 0.095|
+---------+------------------------+-------------------+----+-----------+---------+-----------+------+
```

In Panel A, the relationship between prior-year common share repurchases and next-year return on common equity (ROE) was close to zero ($r = -0.049$, $p = 0.858$; $\rho = -0.035$, $p = 0.897$, $N = 16$). In this sample, the near-zero association provides little evidence of a systematic positive relationship between prior-year repurchases and next-year ROE.

In Panel B, prior-year share repurchases showed a negative association with next-year operating margins ($r = -0.403$, $p = 0.194$; $\rho = -0.385$, $p = 0.217$, $N = 12$). This negative association coincided with peak share buybacks in 2021 and a subsequent decline in operating margins in 2022. This timing pattern is strictly observational and does not establish an economic explanation or a causal relationship.

In my view, these different empirical patterns suggest that the same broad capital-allocation variable may appear differently across firms with different structures. Because the sample size is small and the design is observational, these calculations represent exploratory patterns rather than proof of any underlying causal link.

---

## 5.2 Why the Same Financial Variable May Have Different Meanings

A central idea that emerged from this project is that a financial variable cannot be evaluated in isolation from the organization that produces it. Across the two panels, financial measures that share similar names often carry very different practical meanings because of differences in:
1. **Business Model**
2. **Financial Structure**
3. **Regulatory Environment**
4. **Operating Structure**

The table below summarizes these structural contrasts across the two panels:

| Dimension | Panel A: Bank Holding Companies | Panel B: Advisory Boutiques |
| :--- | :--- | :--- |
| **Balance-Sheet Asset Characteristics** | Large balance sheets with loans, trading inventory, and securities | Asset-light balance sheets ($1B–$5B in assets) with minimal inventory |
| **Primary Business Focus** | Integrated banking: commercial lending, deposit-taking, market-making, and underwriting | Advisory services: M&A advice, restructuring, capital raising, and asset management |
| **Regulatory Capital Regime** | Federal Reserve Basel III framework: Standardized CET1, Tier 1 Leverage, and SLR | SEC net capital rules for broker-dealer subsidiaries; corporate capital at parent level |
| **Primary Operating Cost** | Interest expense, technology infrastructure, credit provisions, and personnel | Personnel compensation and benefits (typically 55% to 70% of net revenue) |
| **Funded Debt Structure** | Substantial long-term senior and subordinated debt funding earning assets | Zero funded debt (Evercore, Moelis) or senior notes (Lazard) alongside cash cushions |
| **Primary Steering Metric** | Return on Common Equity (ROE), Standardized CET1, Efficiency Ratio | Compensation Expense Ratio, Operating Margin, Advisory Revenue |

Consider the meaning of "capital" in each panel:
- In **Panel A**, capital is defined primarily through statutory regulatory ratios such as Standardized CET1, which ranged between 13.1% and 17.4% during 2020–2024. Regulatory capital requirements provide an important institutional context for interpreting bank holding company capital ratios.
- In **Panel B**, advisory firms operate asset-light balance sheets without bank regulatory capital requirements. Capital allocation is observed through cash liquidity reserves ($274M to $688M in net cash at Evercore and Moelis in 2024), shareholder distributions, and operating expenditures.

These structural differences mean that the same financial variable should be interpreted within the specific environment in which it was generated. It would be misleading to compare a bank holding company's balance-sheet equity directly with an advisory boutique's equity. Importantly, acknowledging these structural differences is an interpretive observation; it does not claim that business model or regulatory framework determined any particular observed result.

---

## 5.3 Decision-Making and Capital Allocation

To make sense of how external conditions relate to observable financial outcomes, I developed a conceptual chain that connects financial conditions to observable data through firm decision-making:

```
+-------------------------------------------------------------+
|                     FINANCIAL CONDITIONS                    |
|   (Macro deal cycles, interest rates, regulatory rules,     |
|              market volatility, fee revenue)                |
+-------------------------------------------------------------+
                              |
                              v
+-------------------------------------------------------------+
|          POSSIBLE DECISION-MAKING CONSIDERATIONS            |
|   (Unobserved factors: risk tolerance, talent retention,    |
|      balance-sheet considerations, liquidity needs, etc.)   |
+-------------------------------------------------------------+
                              |
                              v
+-------------------------------------------------------------+
|                 CAPITAL-ALLOCATION DECISIONS                |
|   (Setting dividend rates, executing share repurchases,     |
|      allocating compensation pools, retaining capital)      |
+-------------------------------------------------------------+
                              |
                              v
+-------------------------------------------------------------+
|                  OBSERVABLE FINANCIAL OUTPUTS               |
|      (Cash dividends paid, common share buybacks, CET1,     |
|      compensation ratios, operating margins, ROE)           |
+-------------------------------------------------------------+
```

In this framework, observable data—such as cash dividends paid, shares repurchased, reported CET1 ratios, compensation ratios, and return on equity—represent **financial outputs**. These outputs may reflect how firms navigate financial conditions through their decision-making processes. Possible decision-making considerations could include risk tolerance, talent retention, liquidity needs, balance-sheet considerations, and shareholder expectations. However, these factors are not directly measured in this study.

For example, when net revenues expanded during the 2021 transaction boom, firms in both panels reported higher net income. How that revenue coincided with observable outputs differed across the two panels:
- Bank holding companies reported changes in retained capital, asset bases, and share repurchases over the same period.
- Advisory boutiques reported changes in compensation expenditures, dividends, and share repurchases as revenues changed across the study period.

When market conditions reversed in 2022–2023, the observable outputs adjusted: share repurchases contracted sharply across both panels, while regular cash dividends continued to be paid.

**Crucial Epistemic Limitation**:
The SEC Form 10-K filings used in this study record numerical outputs, such as dollars spent and ratios reported. They do not record boardroom discussions, executive debates, or internal strategy memos. Because decision-making considerations are not directly observed in the data, this conceptual chain must be understood as an interpretive framework proposed by the researcher, not as an established empirical finding.

---

## 5.4 Dividends, Repurchases and Different Forms of Capital Distribution

Over the five-year period from 2020 through 2024, the eight candidate firms returned an aggregate of **$233.2 billion** to equity holders:
- **Cash Dividends Paid**: $113.8 billion (48.8% of total distributions)
- **Common Share Repurchases**: $119.3 billion (51.2% of total distributions)

While the total dollars returned were almost evenly split between dividends and repurchases over the full period, the longitudinal patterns of these two distribution channels differed markedly:

1. **Dividend Stability**: Annual cash dividends followed a steady or upward path throughout the cycle. From 2020 to 2024, annual dividend payments grew by +92.5% at Goldman Sachs ($1,254M to $2,414M), +124.1% at Morgan Stanley ($999M to $2,239M), +16.5% at JPMorgan Chase ($10,950M to $12,757M), and +208.0% at Stifel Financial ($50M to $154M). Even during the 2022–2023 revenue downturn, regular dividend payments were maintained or increased across all firms.
2. **Repurchase Variation**: In contrast to dividends, share repurchases showed large annual swings that aligned with revenue conditions. In 2021, when advisory and underwriting fees reached historic highs, common share repurchases expanded dramatically to $18,449M at JPMorgan Chase (up from $6,456M in 2020) and $11,540M at Morgan Stanley (up from $1,280M in 2020). During the 2022–2023 downturn, share buybacks contracted steeply before recovering in 2024.

This comparison provides a clear empirical example of how related financial variables within the same broad category—shareholder distributions—can behave in fundamentally different ways.

In interpreting this difference, it is important to avoid attributing conscious motives to corporate management. We cannot state that "management deliberately used buybacks as a flexible buffer." A more careful and accurate statement supported by the data is:

> *The observed pattern is consistent with dividends functioning as a recurring payout component, while repurchases varied more across years.*

---

## 5.5 Regulatory Constraints and Business Model Differences

The comparison between bank holding companies and independent advisory boutiques highlights that capital-allocation measures should not automatically be interpreted in the same way across different business models.

### Panel A: Bank Holding Companies and Regulatory Solvency
Bank holding companies operate within a comprehensive regulatory system overseen by the Federal Reserve, the OCC, and the FDIC. Under Basel III rules:
- Firms are required to maintain minimum Standardized Common Equity Tier 1 (CET1) capital ratios to protect against unexpected balance-sheet losses. In this study, reported CET1 ratios ranged between 13.1% and 17.4% from 2020 to 2024.
- Capital distributions are subject to annual supervisory stress testing (such as the Comprehensive Capital Analysis and Review, or CCAR). A bank holding company cannot freely distribute capital without ensuring that its projected post-stress capital ratios satisfy regulatory minimums.
- Leverage constraints, including the Supplementary Leverage Ratio (SLR), place an upper boundary on total balance-sheet exposure relative to Tier 1 capital.

Because of these rules, capital retention for a bank holding company is closely tied to legal solvency mandates and balance-sheet capacity.

### Panel B: Advisory Boutiques and Expense Flexibility
Independent advisory boutiques operate under an entirely different economic model:
- They do not take customer deposits, provide commercial loans, or finance multi-billion-dollar trading inventories.
- Their largest single operating expense is personnel compensation, which averaged 63.5% to 65.4% of net revenues over the study period.
- During the 2023 deal downturn, advisory compensation ratios increased to cycle highs (66.0% at Evercore, 70.0% at Moelis, and 71.6% at Lazard), while operating margins contracted (5.1% to 15.0%). The data show that compensation ratios increased while revenue declined during the 2023 downturn.
- Instead of regulatory capital ratios, boutiques maintained liquidity through net cash cushions ($274M to $688M in 2024 at Evercore and Moelis) and zero funded long-term debt.

### Principle of Business Model Neutrality
These observations suggest that similar capital-allocation measures can have different operational meanings across the two business models:
- In bank holding companies, capital is defined primarily through retained equity and regulatory capital ratios that operate under regulatory supervision.
- In advisory boutiques, capital allocation is observed through cash liquidity reserves alongside distributions and operating expenditures.

This distinction does not imply that one business model is preferable to or better structured than another. Both business models represent coherent institutional structures designed to support different activities within the financial sector.

---

## 5.6 Limitations and Alternative Explanations

To ensure transparency and intellectual honesty, this study must be evaluated alongside its limitations and possible alternative explanations.

### 1. Small Sample Size
The exploratory lagged analysis ($t \to t+1$) contains only four annual transitions per firm over the five-year period. This limits the sample size to:
- Maximum $N = 16$ for Panel A (4 firms $\times$ 4 transitions)
- Maximum $N = 12$ for Panel B (3 firms $\times$ 4 transitions)

With sample sizes this small, correlation coefficients and $p$-values cannot be interpreted as statistically definitive. A single firm's unique experience in one transition can heavily influence the calculated coefficient.

### 2. Five-Year Time Period (2020–2024)
The five-year study period captured extraordinary macroeconomic volatility, including the initial COVID-19 pandemic shock in 2020, the historic underwriting boom of 2021, and the rapid 525-basis-point interest-rate tightening cycle in 2022–2023. While this volatility provided rich variation, five years is a comparatively short window that cannot evaluate multi-decade capital cycles.

### 3. Observational Study Design
This project is strictly observational. It does not employ randomized experiments, natural experiments, or instrumental variables. Consequently, no finding in this report can establish cause and effect.

### 4. No Direct Measurement of Management Decision-Making
SEC Form 10-K filings provide audited accounting measures, but they do not record the internal deliberations, risk tolerances, or strategic debates of executive teams. Any discussion of decision-making must remain an interpretive hypothesis rather than an observed fact.

### 5. Unobserved Variables
Many factors that influence firm performance are not captured in standardized financial filings, including client relationship strength, banker recruitment and departures, deal pipeline depth, and internal risk-management models.

### 6. Common Market Movements
Because revenues, margins, and returns moved in similar directions across all eight firms between 2020 and 2024, broad market-wide conditions coincided with large shared fluctuations in operating performance. The data cannot cleanly separate common market movements from firm-level capital-allocation effects.

### 7. Business Model Differences Within Panels
Even within panels, firms are not completely homogeneous:
- In Panel A, JPMorgan Chase possesses a massive consumer deposit franchise, Stifel has an extensive retail wealth-management network, and Goldman Sachs remains more reliant on global markets and investment banking.
- In Panel B, Lazard operates an established global asset-management business alongside its financial advisory arm, whereas Evercore and Moelis operate primarily as pure advisory firms.

### 8. Possible Timing Effects in Advisory Revenues
In Panel B, lagged investment-banking revenue in year $t$ showed a moderate positive association with next-year operating income ($t+1$) ($r = +0.470$, $p = 0.123$; $\rho = +0.503$, $p = 0.095$, $N = 12$).

One possible explanation is that advisory transactions can span more than one fiscal period, but this study does not contain deal-level timing data to test that explanation. Therefore, deal timing must be viewed as an untested hypothesis rather than an established empirical finding.

---

## Conclusion

This independent research project explored the capital allocation practices of eight major U.S. investment-banking and financial advisory firms over the five-year period from 2020 through 2024.

### 1. What Did the Study Examine?
The study examined primary financial data collected from 40 official SEC Form 10-K filings to evaluate how firms distributed capital to shareholders, retained equity on their balance sheets, and experienced subsequent operating performance across two distinct business models: bank holding companies (Panel A) and independent advisory boutiques (Panel B).

### 2. What Was Observed?
Across 2020–2024, the empirical data revealed:
- An aggregate of **$233.2 billion** returned to shareholders ($113.8B in cash dividends and $119.3B in share repurchases).
- Consistently stable or increasing annual cash dividends alongside highly variable annual share repurchases.
- Bank holding company Standardized CET1 ratios that remained between 13.1% and 17.4%, consistently exceeding regulatory minimums.
- Advisory boutique compensation ratios that rose to 66%–71% during the 2023 revenue downturn, while operating margins contracted.
- Markedly different exploratory lagged association patterns across panels, including a near-zero relationship between prior-year repurchases and next-year ROE in Panel A ($r = -0.049$, $p = 0.858$, $N = 16$), and a negative association between prior-year repurchases and next-year operating margins in Panel B ($r = -0.403$, $p = 0.194$, $N = 12$).

### 3. What Interpretation Does the Researcher Take?
Reflecting on these findings, my central interpretation as an independent student researcher is:

> **The main insight I take from this study is that financial outputs may reflect the interaction between financial conditions and the mechanisms through which firms make capital-allocation decisions.**

From this perspective:
- The different correlation patterns observed across the two panels suggest that the same financial variable may not carry the same economic meaning or function across different types of firms.
- Business model, financial structure, and regulatory environment may help explain why similar financial variables appear differently across the two panels.
- Firm decision-making may provide one possible connecting link between changing financial conditions and observable financial outputs.

### 4. What Can the Study Not Establish?
It is equally important to be clear about what this study cannot determine:
- Decision-making processes are not directly observed in financial statements.
- The analysis cannot establish causal relationships or verify management motives.
- The small sample sizes ($N = 12$ to $16$) mean all statistical associations are exploratory.
- The data does not provide a basis for ranking business models or claiming that one capital allocation strategy was superior to another.

---

## Author Research Perspective & Reflection Scaffolding

As the student author, I maintained this framework to separate my personal reflections from the factual data analysis. Below is my research reflection scaffold:

- **My interpretation**:  
  [SHORT PLACEHOLDER: The student author will insert their personal overall interpretation of the findings here.]

- **What I think is most important**:  
  [SHORT PLACEHOLDER: The student author will describe what they view as the central takeaway of the study.]

- **What surprised me**:  
  [SHORT PLACEHOLDER: The student author will explain which empirical result was most unexpected.]

- **One result I would interpret cautiously**:  
  [SHORT PLACEHOLDER: The student author will identify which correlation or trend requires the greatest caution.]

- **One question I would investigate in a future project**:  
  [SHORT PLACEHOLDER: The student author will state their proposed next research question.]
