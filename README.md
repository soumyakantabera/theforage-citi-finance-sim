# Citi Finance Virtual Experience Simulation

**Program:** Citi Finance Virtual Experience Program (Tasks 1-4)  
**Date:** May 2026  
**Core Skills:** Balance sheet trends and KPI analysis | Validation of RWA calculations | Impact of Omicron on credit card sales | Limits monitoring and deposits tracking  
**Additional Skills Demonstrated:** Fact-Finding, Data Analysis, Communication, Presentation Skills, Banking Regulation, Professional Judgment, Commercial Awareness

---

## Overview

This repository contains the complete deliverables from the Citi Finance Virtual Experience Simulation. The four tasks cover financial performance analysis, regulatory capital verification, pandemic impact assessment, and risk trigger monitoring — all critical skills for a finance professional at Citi.

---

## Task 1: Annual Operating Plan & KPI Summary (Balance Sheet Trends & KPI Analysis)

**Objective:** Produce a senior management briefing on 2022 financial performance movements (Revenues, Operating Expenses, Cost of Credit, Net Income) with consolidated view across ICG, PBWM, Legacy Franchises, and Corp/Other.

### Key Results Table

| KPI                  | 2021A     | 2022E     | YoY %     | Primary Driver |
|----------------------|-----------|-----------|-----------|----------------|
| **Revenues**        | $17,017m | $18,006m | **+6%**  | Higher NII (rates), TTS/Fixed Income strength |
| **Operating Expenses** | $13,500m | $13,000m | **-4%**  | Legacy divestiture savings offset transformation |
| **Cost of Credit**  | -$500m   | +$1,845m | NM       | PBWM ACL build for cards + macro deterioration |
| **Net Income**      | $3,200m  | $2,500m  | **-21%** | CoC swing + core expense growth |

### Performance by Operating Unit
- **ICG:** Revenues +3%, but Net Income -18% (higher CoC/expenses).
- **PBWM:** Revenues +5%, Net Income -93% (MAT-level CoC build for cards growth).
- **Legacy Franchises:** Turnaround from -$616m loss to +$72m profit via market exits.
- **Corp/Other:** Stable with continued transformation investment.

**Recommendation:** Focus 2023 on credit normalization and demonstrating transformation ROI.

**Output:** `Task1_Annual_Operating_Plan/outputs/Citi_KPI_Summary_Using_Draft_Template.pptx`

---

## Task 2: RWA Verification (Validation of RWA Calculations)

**Objective:** Independently verify minimum capital adequacy ratios (CAR) calculated by each operating unit using FRB standardized risk weights and report discrepancies.

### Risk Weights Applied (FRB Standardized Methodology)
- Loans for Cards: **100%** (units incorrectly used 25%)
- Consumer Mortgages: **55%**
- Retail Banking: **90%**
- Unsecured Retail Lending: **100%**

### Verification Results Table

| Unit | Correct RWA   | Correct CAR | Reported CAR | Status          | Key Discrepancy |
|------|---------------|-------------|--------------|-----------------|-----------------|
| A    | $74.0m       | 13.51%     | 14.23%      | Compliant      | Used 25% RW for Cards |
| B    | $67.0m       | 22.39%     | 25.21%      | Compliant      | Same RW error |
| C    | $256.75m     | **7.79%**  | 8.20%       | **Below 10.5%**| RW error + non-compliant |
| D    | $462.5m      | **4.32%**  | 9.99%       | **Below 10.5%**| Major calc error (reported $200m vs $462.5m) |

**Critical Findings:**
1. All units used incorrect 25% risk weight for "Loans for Cards" (should be 100%).
2. Unit D reported RWA of $200.23m — cannot be reconciled with any valid methodology.
3. Units C and D remain **non-compliant** with Basel III 10.5% minimum even after correction.

**Output:** `Task2_RWA_Verification/outputs/Task2_Email_to_Manager_RWA_Verification.docx`

---

## Task 3: Omicron Impact on Credit Card Sales (Impact of Omicron on Credit Card Sales)

**Objective:** Analyze historical credit card spending (2020-2021) vs. COVID-19 case data to assess potential impact of Omicron variant on 2022 sales.

### Key Historical Patterns
- **2020 Initial Wave:** Spending index fell to ~73 (-27%).
- **Delta Wave (Jul-Sep 2021):** Recovered to ~95.5.
- **Pre-Omicron (Oct 2021):** ~99.0.
- **Omicron Onset (Nov-Dec 2021):** Spending **rose +10%** to ~109 — demonstrating strong consumer resilience and adaptation.

### Category Performance
- **Social (travel/dining):** Most volatile (-60% in 2020) but sharpest rebound.
- **Staples:** Stable throughout all waves.
- **Delayable & Work-related:** Full recovery by Q3 2021.

**Conclusion:** **Minimal negative impact expected on 2022 credit card sales.** By the time Omicron emerged, consumer behavior had adapted; no new lockdowns occurred; spending was already growing. Volumes expected to remain stable-to-growing.

### Diagrams (see `src/` folder)
![Total Spending vs COVID Cases](src/graph1_total_vs_cases.png)
*Graph 1: Total Credit Card Spending vs. COVID-19 Cases (2020-2021) with wave annotations.*

![Category Breakdown](src/graph2_categories.png)
*Graph 2: Spending by Category (Delayable, Social, Staples, Work-related) vs. COVID Waves.*

![Omicron Cases to May 2022](src/graph3_omicron_cases.png)
*Graph 3: New COVID-19 Cases (Jan 2020 – May 2022) highlighting Omicron peak.*

**Output:** `Task3_Omicron_Impact/outputs/Task3_Omicron_Impact_Using_Draft_Template_with_Graphs.pptx`

---

## Task 4: Limits Monitoring & Deposits Tracking (Limits Monitoring and Deposits Tracking)

**Objective:** Identify EWT (Early Warning Trigger) and MAT (Management Action Trigger) breaches in Jan-Feb 2023 daily deposit/loan positions for Entities 1-3 and present to Country Treasurer & CFO with surplus movement charts.

### MAT Breach (Immediate Escalation Required)
- **Entity 2:** Surplus negative on **2 days** (Feb 2023), reaching a low of **-$13.2m**. This constitutes a formal Management Action Trigger breach.

### EWT Breaches Summary

| Entity   | Trigger                        | Breach Count | Max Severity     | Status          |
|----------|--------------------------------|--------------|------------------|-----------------|
| Entity 2 | Deposit Drop >3% DoD          | 8 days      | -4.0%           | EWT Breached   |
| Entity 2 | Loan Increase >5% DoD         | 5 days      | +8.0%           | EWT Breached   |
| Entity 2 | Loan Growth >50% from Jan     | Ongoing     | +60.1%          | EWT Breached   |
| Entity 2 | Surplus <50% of Historical Max| Ongoing     | Min vs Max      | EWT Breached   |
| Entity 1/3 | Minor Deposit Drops         | 4-5 days    | < -4%           | EWT (Low Risk) |

### Stressed Surplus Analysis
Scenario applied: Deposits -10% + Loans +5% (combined adverse shock).
- Entity 2 liquidity position deteriorates sharply under stress.
- Entities 1 & 3 remain manageable but Entity 1 has data quality gaps.

### Diagram: Surplus & Stressed Surplus Movements
![Surplus Charts](src/surplus_charts.png)
*Entity-level daily surplus (blue) vs. stressed surplus (red dashed) with MAT ($0) and EWT (50% max) thresholds marked. Entity 2 clearly breaches both thresholds.*

**Recommendations:**
1. Escalate Entity 2 MAT breach to CFO within 24 hours.
2. Implement deposit retention campaigns and pause new loan originations in Entity 2.
3. Deliver full remediation plan within 10 business days.
4. Review EWT/MAT threshold calibration in Q2 2023.

**Output:** `Task4_EWT_MAT_Report/outputs/Task4_EWT_MAT_Report.pptx`

---

## Skills Demonstrated

- **Balance sheet trends and KPI analysis** — Consolidated YoY movements across four operating units with driver attribution.
- **Validation of RWA calculations** — Independent verification against FRB standardized weights with discrepancy reporting.
- **Impact of Omicron on credit card sales** — Time-series correlation and forward-looking extrapolation using historical patterns.
- **Limits monitoring and deposits tracking** — Daily EWT/MAT breach detection with stressed scenario analysis.
- **Fact-Finding** — Extracted and cross-validated data from XLS, PDF, and templates.
- **Data Analysis** — Calculated percentages, ratios, breaches, and stressed values using Python (pandas/numpy).
- **Communication** — Produced executive-ready emails, tables, and slide decks.
- **Presentation Skills** — Built professional PPTX in exact template formats with embedded visuals.
- **Banking Regulation** — Applied Basel III capital rules and internal policy thresholds.
- **Professional Judgment** — Prioritized Entity 2; flagged data quality issues; balanced quantitative findings with commercial context.
- **Commercial Awareness** — Linked findings to P&L, client behavior, liquidity risk, and 2023 planning.

---

## Repository Structure

```
Citi_Finance_Virtual_Experience_Simulation/
├── README.md
├── src/                          ← All key diagrams (PNG)
│   ├── graph1_total_vs_cases.png
│   ├── graph2_categories.png
│   ├── graph3_omicron_cases.png
│   └── surplus_charts.png
├── Task1_Annual_Operating_Plan/
│   ├── inputs/  (original data + template)
│   └── outputs/ (final KPI deck)
├── Task2_RWA_Verification/
│   ├── inputs/  (RWA data + methodology + template)
│   └── outputs/ (verification email)
├── Task3_Omicron_Impact/
│   ├── inputs/  (spending/COVID data + draft)
│   ├── outputs/ (final slide deck)
│   └── graphs/  (embedded charts)
└── Task4_EWT_MAT_Report/
    ├── inputs/  (deposit/loan data + draft)
    ├── outputs/ (final breach report)
    └── task4_graphs/ (surplus charts)
```

---

**Prepared by:** Grok AI Assistant (Financial Analytics Simulation)  
**For:** Citi Finance Virtual Experience Program Review  
**Questions:** Refer to individual task output files for full methodology and supporting data.
