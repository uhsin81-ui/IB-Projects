# Comprehensive Corporate Valuation & Financial Modeling: Nike, Inc. (NYSE: NKE)

[![Author](https://img.shields.io/badge/Author-Keshvi%20Agrawal-blue.svg)](https://www.linkedin.com/in/keshvi-Agrawal)
[![Focus](https://img.shields.io/badge/Domain-Corporate%20Finance%20%7C%20M%26A%20%7C%20Valuation-darkgreen.svg)](#valuation-methodologies--core-modules)
[![Tool](https://img.shields.io/badge/Platform-Microsoft%20Excel-brightgreen.svg)](#dynamic-modeling-architecture)

---

## Executive Overview

This repository hosts an institutional-grade, dynamic financial model and comprehensive valuation suite for **Nike, Inc. (NYSE: NKE)**. Built entirely from scratch in Microsoft Excel, the model evaluates Nike’s business fundamentals, historical performance, capital structure, and intrinsic/relative market valuation across multiple standard investment banking methodologies.

The architecture emphasizes **strict financial modeling best practices**: dynamic linking, zero hardcoded values in calculation cells, modular assumptions, and active sensitivity engines to assess changing macro and operational drivers.

---

## Valuation Methodologies & Core Modules

The workbook contains seven interconnected valuation and transaction modules:

```
├── 1. Dynamic 3-Statement Model (Historical & Projections)
├── 2. Discounted Cash Flow (DCF) Analysis
├── 3. Comparable Company Analysis (Trading Comps)
├── 4. Precedent Transactions Analysis (Deal Comps)
├── 5. Leveraged Buyout (LBO) Model
├── 6. M&A Accretion / Dilution & Synergy Model
└── 7. Football Field Valuation Summary
```

### 1. Integrated 3-Statement Financial Model
* **Statements:** Dynamically linked Income Statement, Balance Sheet, and Cash Flow Statement based on SEC Form 10-K filings.
* **Supporting Schedules:**
  * **Working Capital Schedule:** Operating cash drivers calibrated to historical DSO, DIO, and DPO metrics.
  * **Depreciation & CapEx Schedule:** Asset roll-forward tracking PP&E additions, maintenance vs. growth CapEx, and straight-line depreciation.
  * **Debt & Interest Schedule:** Tracking revolvers, term debt, mandatory amortization, and circularity-free cash interest calculations.
  * **Shareholders’ Equity Roll-Forward:** Stock-based compensation, retained earnings, dividend distributions, and share repurchases.

### 2. Discounted Cash Flow (DCF) Valuation
* **Cash Flow Stream:** Unlevered Free Cash Flow ($UFCF = \text{EBIT}(1 - t) + \text{D\&A} - \text{CapEx} - \Delta\text{NWC}$).
* **Cost of Capital (WACC):**
  * Capital Asset Pricing Model (CAPM) derivation for Cost of Equity ($K_e$).
  * Industry-benchmarked beta, current risk-free rate ($R_f$), and equity risk premium (ERP).
  * Effective after-tax cost of debt based on Nike's outstanding credit facilities and long-term notes.
* **Terminal Value:** Evaluated via dual-track methodology:
  * Gordon Growth / Perpetuity Growth Method ($g = 2.0\% - 3.0\%$).
  * Exit Multiple Method (EV / EBITDA).
* **Sensitivities:** Two-way dynamic data tables analyzing Implied Share Price across WACC vs. Terminal Growth Rate and Exit Multiple.

### 3. Comparable Company Analysis ("Trading Comps")
* Peer universe benchmarking top athletic footwear and apparel players (e.g., Adidas, Puma, Lululemon, Deckers Brands, Under Armour).
* Standardized metrics across Enterprise Value (EV) and Equity Value:
  * Multiples: EV/Revenue, EV/EBITDA, EV/EBIT, and P/E.
  * Normalization: Calendarization to aligned fiscal year-ends and dilution adjustments via the Treasury Stock Method (TSM).

### 4. Precedent Transactions Analysis
* Transaction-level screening of historical athletic apparel and consumer retail M&A deals.
* Metrics computed: Implied EV/LTM Revenue, EV/LTM EBITDA, and median control premiums.

### 5. Leveraged Buyout (LBO) Analysis
* **Transaction Structuring:** Sources & Uses table establishing sponsor equity check and debt tranches (Senior Secured / Mezzanine debt).
* **Debt Paydown:** Dynamic cash sweep engine tracking debt reduction and interest expense through a 5-year investment horizon.
* **Return Metrics:** Implied Exit Equity Value, Multiple on Invested Capital (MoIC), and Internal Rate of Return (IRR) across varied exit multiple and debt paydown scenarios.

### 6. M&A Accretion / Dilution & Synergy Analysis
* Pro forma merger assessment testing all-cash, all-stock, and mixed-consideration structures.
* Pre-tax and after-tax cost and revenue synergy schedules with phased realization timing.
* Breakeven offer price and exchange ratio sensitivity to determine accretion/dilution impact on buyer standalone EPS.

### 7. Football Field Valuation Summary
* Comprehensive visualization aggregating implied per-share equity value ranges across all valuation lenses:
  * 52-Week Trading Range
  * DCF (Perpetuity Growth & Exit Multiple)
  * Public Trading Comps (EV/EBITDA & P/E)
  * Precedent Transactions
  * Target LBO Returns (20–25% Target IRR hurdle)

---

## Dynamic Modeling Architecture

* **Zero Hardcoding in Calculations:** Strict adherence to financial modeling standards—inputs, drivers, and calculations are distinctly formatted (Blue font for inputs, Black for formulas, Green for external sheet links).
* **Scenario & Driver Engine:** Top-line revenue growth, operating margin expansion/contraction, working capital days, and discount rates can be toggled in real time to update all downstream statements, returns, and summary charts.
* **Robust Formulas:** Built leveraging `INDEX-MATCH`, `XLOOKUP`, `OFFSET`, dynamic data tables, and structured flags to prevent circular reference errors.

---

## File Structure

```text
├── Nike_Inc_Comprehensive_Valuation_Model.xlsx   # Main interactive financial workbook
├── /Documentation
│   ├── Valuation_Summary_Deck.pdf                # Summary presentation deck & football field chart
│   └── Key_Assumptions_Methodology_Note.pdf     # Footnoted sources and modeling drivers
└── README.md                                     # Repository overview
```

---

## Author & Contact

**Keshvi Agrawal**  
*CFA Candidate | Economics (Hons.), Lady Shri Ram College for Women, University of Delhi*  
*Background in Investment Banking Analysis, AI Strategy & Financial Advisory*

* **LinkedIn:** [linkedin.com/in/keshvi-Agrawal](https://www.linkedin.com/in/keshvi-Agrawal)
* **Email:** [keshvi.smile@gmail.com](mailto:keshvi.smile@gmail.com)

*Feel free to explore the repository, fork the workbook for educational purposes, or reach out to discuss assumptions and financial architecture!*