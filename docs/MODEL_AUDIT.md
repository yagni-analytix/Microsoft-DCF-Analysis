# Model Audit Report

**Prepared for:** Yagni Patel

## Audit conclusion

**Status: PASS**

The uploaded workbook was rebuilt and reviewed for source consistency, financial-model logic, formula integrity, comparability, valuation mechanics, and presentation quality. The final version contains no detected `#REF!`, `#DIV/0!`, `#VALUE!`, `#NAME?`, or `#N/A` errors in the key model ranges.

## Material corrections

| Area | Issue identified | Correction | Valuation / analytical impact |
|---|---|---|---|
| Risk-free rate | Prior model used 4.10% for the August 6, 2026 valuation date | Updated to 4.69%, the dated 10-year Treasury constant-maturity rate | WACC increased to 9.47% |
| Base DCF | Valuation reflected the lower WACC | Recalculated explicit and terminal cash flows | Value changed to $367.85 per share |
| Reverse DCF | Prior solved uplift reflected the earlier valuation inputs | Re-solved against corrected market-implied enterprise value | Uplift changed to 7.41 pp |
| Segment history | Legacy and recast data could be interpreted as a continuous series | FY2023A-FY2026A designated as FY2025-recast basis; FY2021A-FY2022A separated | Prevents false growth and margin conclusions |
| FY2022 segment basis | Revenue and operating-income figures had mixed reporting bases | Standardized FY2022 legacy-basis figures | Corrected segment margins |
| Capital allocation | Mixed authorized/declared and cash-flow definitions | Standardized cash spent on share repurchases and cash dividends paid | Improves comparability |
| CapEx treatment | Cash CapEx alone understates infrastructure investment | Added finance-lease additions and Lease-Adjusted UFCF | More conservative and economically complete DCF |
| Invested capital | Current liabilities had previously been treated as debt; finance leases omitted | Rebuilt financing-based invested capital | Corrected ROIC denominator |
| Forecast integrity | Some forecast outputs were hardcoded or inconsistently linked | Replaced with formulas tied to assumptions | Improves auditability and scenario responsiveness |
| DCF dates | Terminal/explicit timing used inconsistent treatment | Applied Actual/Actual YEARFRAC and mid-year convention | Corrected discounting |
| Share count | 7,453 million was described as shares outstanding | Relabeled as FY2026 diluted weighted-average proxy | Avoids misleading point-in-time claim |
| Decision framework | Quantitative valuation was not connected to purchase-price discipline | Added Buffett-inspired five-tenet scorecard and margin-of-safety references | Separates company quality from investment attractiveness |
| Narrative output | Workbook lacked a final decision document | Added final investment memo in Markdown, Word, and PDF | Makes the project presentation-ready |
| Author attribution | Prior public-facing materials identified the wrong author | Updated the workbook, README, memo, metadata, and public assets to Yagni Patel | Ensures accurate ownership and attribution |

## Validation performed

- Segment revenue reconciliation
- Segment operating-income reconciliation
- Segment mix reconciliation
- Cash FCF reconciliation
- Average invested-capital validation
- NOPAT and ROIC validation
- Consolidated revenue and operating-income reconciliation
- Cash-Based and Lease-Adjusted UFCF checks
- WACC greater than terminal-growth check
- Equity-value bridge check
- Declining discount-factor check
- Enterprise-value check
- Reverse DCF EV and share-price checks
- Sensitivity base-case tie-out
- Buffett scorecard weighted-point reconciliation
- Final formula-error scan

## Items intentionally retained as assumptions

- Equity risk premium: 4.50%
- Levered beta: 1.10
- Pre-tax cost of debt: 4.50%
- Long-run terminal growth: 3.00%
- Segment growth and operating-margin paths
- D&A, CapEx, and operating-NWC forecast paths
- Buffett-inspired tenet weights and scores

These inputs are clearly identified and should be refreshed or reconsidered when the valuation date changes.

## Remaining optional enhancements

1. Add a treasury-stock-method dilution schedule using options and RSUs.
2. Build fully independent Bear/Base/Bull operating cases.
3. Add quarterly forecast detail for the first two forecast years.
4. Add a structured price-and-volume decomposition for Microsoft 365 and Azure.
5. Add explicit stock-based-compensation dilution analysis.
6. Add a probabilistic Monte Carlo valuation.

These are enhancements, not blockers to presentation.
