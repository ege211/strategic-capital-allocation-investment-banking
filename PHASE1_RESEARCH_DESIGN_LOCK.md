# Phase 1 Research Design Lock: Strategic Capital Allocation in Investment Banking (2020–2024)

**Project Title**: Strategic Capital Allocation in Investment Banking: A Comparative Longitudinal Study of Major U.S. Firms, 2020–2024  
**Author**: 12th-Grade Independent Student Research Project  
**Target Period**: Fiscal Years 2020, 2021, 2022, 2023, and 2024 strictly. (No 2025/2026 data).  
**Phase 1 Status**: **LOCKED**  
**Research Stance**: Observational, longitudinal, cross-firm comparative study. I will not make causal claims (no words like "causes", "drives", "impacts", or "determines"; strictly "associated with", "co-move with", "longitudinal comparison", "subsequent performance").

---

## 1. Research Question

### Core Research Question
> *"How do major investment-banking firms allocate capital between business investment, capital retention, and shareholder distributions, and how are these patterns associated with subsequent business performance?"*

### Refined Analytical Question
> *"To what extent are differences in capital retention and shareholder distribution associated with subsequent operating performance among major investment-banking firms?"*

---

## 2. Conceptual Framework

```
Financial Resources (Revenues, Pre-Tax Cash Flow)
       ↓
Capital Allocation Decisions
       ↓
+-----------------------------+-----------------------------+-----------------------------+
|    Business Investment      |      Capital Retention      |  Shareholder Distributions  |
| (Human Capital, Technology) | (CET1 Buffers, Net Cash)    |   (Dividends, Buybacks)     |
+-----------------------------+-----------------------------+-----------------------------+
       ↓
Subsequent Operating & Financial Performance (ROTCE, Operating Margin, Advisory Growth)
```

---

## 3. Panel Structure

Phase 0 showed that combining diversified bank holding companies (BHCs) and independent advisory boutiques into a single group would create important comparability problems because of their different business models and regulatory rules. Direct comparison across one single table would be difficult and misleading. Therefore, this student research project separates the firms into two main panels and keeps one firm as a separate sensitivity observation.

### Panel A: Regulated Bank Holding Companies (4 Firms)
- **Firms**:
  1. Goldman Sachs Group, Inc. (`GS`)
  2. Morgan Stanley (`MS`)
  3. JPMorgan Chase & Co. (`JPM`)
  4. Stifel Financial Corp. (`SF`)
- **Purpose**: Study capital allocation in large bank holding companies subject to Federal Reserve capital regulations, leverage limits, and stress testing.
- **Core Variables (8 variables)**:
  1. `net_revenue`
  2. `investment_banking_revenue`
  3. `roe_or_rotce`
  4. `efficiency_or_overhead_ratio`
  5. `cet1_standardized`
  6. `tier1_leverage_ratio`
  7. `dividends_paid`
  8. `share_repurchases`
- **Supplementary Descriptive Variables (3 variables)**:
  - `supplementary_leverage_ratio` (reported by GS, MS, JPM; SF is a Category IV bank and is legally exempt from SLR)
  - `tangible_common_equity`
  - `technology_or_business_investment` (operating tech and communications expenses; kept separate as supplementary context)
  *(Note: Supplementary variables provide descriptive context and will not be forced into the main statistical comparisons).*

### Panel B: Independent Advisory Boutiques (3 Firms)
- **Firms**:
  1. Evercore Inc. (`EVR`)
  2. Lazard, Inc. (`LAZ`)
  3. Moelis & Company (`MC`)
- **Purpose**: Study capital allocation in asset-light advisory firms where compensation pools for bankers and direct cash distributions to shareholders are central, rather than Federal Reserve bank capital rules.
- **Core Variables (7 variables)**:
  1. `net_revenue`
  2. `investment_banking_revenue`
  3. `compensation_expense`
  4. `compensation_ratio`
  5. `operating_income`
  6. `operating_margin`
  7. `dividends_and_shareholder_distributions` (cash dividends + share repurchases)
- **Supplementary Descriptive Variables (4 variables)**:
  - `cash`
  - `debt`
  - `net_cash_or_net_debt`
  - `technology_or_business_investment_if_available`
  *(Note: Supplementary variables are retained for descriptive context).*
- **Comparability Notes**:
  - Bank regulatory metrics (CET1, Tier 1 leverage, SLR) do not apply to advisory boutiques and are marked `NOT_APPLICABLE`.
  - Boutiques use partnership structures (Up-C for EVR and MC) or had legacy capital deficits (LAZ), which makes GAAP book ROE structurally non-comparable.

### Extended / Sensitivity Observation: Jefferies Financial Group (`JEF`)
- **Firm**: Jefferies Financial Group Inc. (`JEF`)
- **Separation Reason**:
  1. *Regulatory Status*: Non-BHC broker-dealer holding company under SEC Rule 15c3-1; not governed by Federal Reserve Basel III capital rules.
  2. *Fiscal Year*: Fiscal year ends on **November 30** (a 30-day reporting difference from the December 31 universe).
  3. *Business Model*: Hybrid broker-dealer that also owned legacy merchant-banking businesses during 2020–2022.
- **Rule**: JEF is kept separate for sensitivity checks and descriptive comparisons. It will not be silently combined into Panel A or Panel B.

---

## 4. Common GAAP-Core Layer

To allow careful cross-firm comparison where the accounting rules are truly identical, 5 variables from standard audited financial statements are tracked across all 8 firms:
1. `net_revenue` (from the Income Statement)
2. `investment_banking_revenue` (underwriting and advisory fees)
3. `dividends_paid` (from the Statement of Cash Flows)
4. `share_repurchases` (from the Statement of Cash Flows)
5. `total_cash_returned` (Derived: `dividends_paid + share_repurchases`)

---

## 5. Technology & Business Investment Protocol

Technology expenses (market data feeds, communications, software licenses) are tracked as supplementary descriptive data:
- Moelis (`MC`) does not report a separate technology expense line item (it is bundled into other expenses).
- The other firms report operating technology expenses, but definitions vary.
- Therefore, technology expense is treated carefully as `PARTIAL` and kept separate from primary statistical comparisons.

---

## 6. Student Research Rules

1. **Primary Sources Only**: All data must come directly from official SEC Form 10-K filings.
2. **Clear Provenance**: Every number must have a record showing the exact filing, section, and table it came from.
3. **No Synthetic or Guessed Data**: If a number is not reported, it is marked `UNAVAILABLE`, not guessed.
4. **No Causal Claims**: Use careful language like "was associated with" or "co-moved with".
5. **Exact Five-Year Scope**: Fiscal years 2020 to 2024 only.
