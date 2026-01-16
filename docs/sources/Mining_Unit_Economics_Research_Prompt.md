# Mining Unit Economics: Comprehensive Research Prompt
**For: Ryzen 5700X vs Ryzen 9950X | Denmark 2026-2027 | Verified 1.6 DKK/kWh Electricity**

---

## OBJECTIVE

Conduct a comprehensive, self-validating unit economics analysis for CPU mining two Ryzen configurations in Denmark with verified electricity pricing. This prompt is designed to minimize inconsistencies through explicit variable definition, mandatory source citation, and cross-validation checkpoints.

---

## PART 1: ESTABLISH GROUND TRUTH VARIABLES

**INSTRUCTION: Research and document each variable below. For each, provide:**
1. The value you found
2. The source (with URL or date)
3. Why this specific value applies to Denmark 2026-2027
4. Any assumptions or qualifications

### **A. ELECTRICITY PRICING (USER VERIFIED: 1.6 DKK/kWh average)**

Research the following components and explain how they sum to the 1.6 DKK/kWh average:

```
1. Nord Pool Spot Price (average 2026)
   - FIND: Historical 2025 data to project 2026 average
   - VALIDATE: Cross-check with Energinet.dk forecasts
   - QUESTION: Is 1.6 DKK/kWh realistic for 24-month average?
   
2. System Tariff (fixed)
   - FIND: Energinet.dk official rates 2026
   - VALIDATE: Confirm applies to residential mining
   - DOCUMENT: Annual rate in DKK/kWh
   
3. Nettariff/Distribution (varies by region)
   - FIND: Your specific distributor rate (Copenhagen/Capital region)
   - VALIDATE: Call distributor or check latest tariff card
   - DOCUMENT: Average across peak/off-peak if tiered
   
4. Electricity Tax (el-afgift) 2026-2027
   - FIND: Official government rate (post-January 2026 reduction)
   - VALIDATE: Confirm 24-month duration mentioned
   - CURRENT KNOWN: 0.01 DKK/kWh (January 2026 rate)
   - QUESTION: Does it revert to higher rate after 24 months?
   
5. VAT (25%) Application
   - FIND: Which components are VAT-liable in Denmark?
   - VALIDATE: Does VAT apply to spot, tariffs, tax?
   - CALCULATE: Weighted VAT impact on total rate
   
6. Final Calculation
   - SUM: Spot + tariff + nettariff + tax + VAT = X DKK/kWh
   - COMPARE: Does this equal user's 1.6 DKK/kWh claim?
   - IF DIFFERENT: Explain variance and reconcile
```

**CRITICAL CHECKPOINT #1:**
Before proceeding to revenue calculations, confirm or explain any variance from 1.6 DKK/kWh. If user's rate is correct, document it; if higher/lower, recalculate accordingly.

---

### **B. CPU SPECIFICATIONS & PERFORMANCE METRICS**

**For Ryzen 5700X:**
```
1. Current Market Price (January 2026)
   - FIND: Mindfactory.de, Caseking.de, PriceWatch EU
   - VALIDATE: Multiple sources; take average
   - DOCUMENT: Price in EUR (convert to DKK if needed)
   - NOTE: Use new hardware prices, not used/refurbished
   
2. XMR Mining Hashrate (Monero RandomX)
   - FIND: Official benchmarks (xmrig.com, monero.cc)
   - VALIDATE: Cross-check r/MoneroMining, HashrateLe.com
   - DOCUMENT: Exact KH/s under realistic conditions (not peak)
   - NOTE: Specify if this is sustained or average
   
3. Power Consumption (Measured)
   - FIND: Tom's Hardware reviews, YouTube mining tests (2025-2026)
   - VALIDATE: Multiple sources; check load conditions
   - DOCUMENT: Sustained mining power (not TDP), in Watts
   - CALCULATE: Daily kWh consumption = (Power in W × 24h) / 1000
   
4. Platform Cost (supporting hardware)
   - BREAKDOWN:
     a) Motherboard (AM5, B850 or X870): EUR price
     b) RAM (DDR5 32GB, optimized for RandomX): EUR price
     c) CPU Cooler (AIO 280-360mm): EUR price
     d) PSU (650-750W, 80+ Gold): EUR price
     e) Case: EUR price
     f) Thermal paste, fans, misc: EUR price
   - SOURCE: Same retailers (Caseking, Mindfactory, etc.)
   - TOTAL: Sum all platform costs
```

**For Ryzen 9950X:**
```
(Same process as 5700X for all metrics above)
- Replace part numbers with 9950X equivalents
- Note: 9950X requires better cooling (higher TDP)
- Typical higher-spec cooler + quality PSU may be necessary
- Verify B850-E WIFI or X870-E compatibility & pricing
```

**CRITICAL CHECKPOINT #2:**
Create a comparison table:

| Spec | 5700X | 9950X | Source |
|------|-------|-------|--------|
| CPU Price (EUR) | ? | ? | Mindfactory/Caseking |
| Platform Cost (EUR) | ? | ? | Sum of components |
| Total Capital (EUR) | ? | ? | CPU + Platform |
| XMR Hashrate (KH/s) | ? | ? | Benchmark + verification |
| Sustained Power (W) | ? | ? | Measured mining load |

If any data is missing or inconsistent, flag it before proceeding.

---

### **C. CRYPTOCURRENCY REVENUE (MONERO/KASPA/AUXILIARY)**

**XMR (Monero) Revenue:**
```
1. Current XMR Price (January 2026)
   - FIND: CoinGecko, CoinMarketCap (current live price)
   - VALIDATE: Multiple sources
   - DOCUMENT: Price in EUR (not USD)
   - NOTE: Use current price; do NOT project future price changes
   
2. Mining Pool Fee & Payout Structure
   - FIND: SupportXMR.com, MoneroHash.com fee structure
   - VALIDATE: Official pool website documentation
   - DOCUMENT: Pool fee percentage (typical 0.6%)
   - CALCULATE: Effective revenue = (XMR earned × price) × (1 - pool fee)
   
3. Daily XMR Revenue Per KH/s
   - RESEARCH: r/MoneroMining recent earnings posts (2026)
   - OR: Use formula: Difficulty adjustment → revenue/day
   - VALIDATE: Cross-check against pool statistics
   - DOCUMENT: EUR/day earned per KH/s
   - CALCULATE: 5700X daily revenue = 10.3 KH/s × (EUR/KH/s/day)
   - CALCULATE: 9950X daily revenue = 28 KH/s × (EUR/KH/s/day)
```

**Merged Mining (Auxiliary Coins):**
```
1. Mergeable Chains (January 2026)
   - FIND: Current list of coins merge-mined with XMR
   - VALIDATE: Check pool support (SupportXMR, P2Pool, MoneroHash)
   - DOCUMENT: Which chains available (VRSC, DERO, others?)
   
2. Per-Chain Revenue (realistic)
   - FOR EACH CHAIN:
     a) RESEARCH: Current mining revenue/day
     b) VALIDATE: Pool statistics or calculator
     c) DOCUMENT: EUR/day expected
   
3. Total Merged Mining Uplift
   - CALCULATE: Sum of all auxiliary chains' daily revenue
   - EXAMPLE: VRSC €0.15/day + other €0.10/day = €0.25/day uplift
   - VALIDATE: Cross-check against recent mining data
   - NOTE: This may vary; document your specific chain choices
   
4. Merged vs. Solo Comparison
   - 5700X solo: ? EUR/day (XMR only)
   - 5700X merged: ? EUR/day (XMR + auxiliary)
   - Uplift percentage: (merged - solo) / solo × 100%
   - Same for 9950X
```

**CRITICAL CHECKPOINT #3:**
Create revenue table (daily, then annualized):

| Revenue Type | 5700X (EUR/day) | 9950X (EUR/day) | Source |
|--------------|-----------------|-----------------|--------|
| XMR only | ? | ? | Mining calculation |
| Merged uplift | ? | ? | Pool data |
| Total daily | ? | ? | Sum |
| Annual (×365) | ? | ? | Daily × 365 |

---

### **D. COSTS: ELECTRICITY + MAINTENANCE + OVERHEAD**

**Annual Electricity Cost:**
```
1. For 5700X:
   - Power consumption: ? W (from Checkpoint #2)
   - Daily kWh: (W × 24) / 1000
   - Annual kWh: Daily kWh × 365
   - Electricity rate: 1.6 DKK/kWh (USER VERIFIED)
   - Annual DKK cost: Annual kWh × 1.6 DKK
   - Convert to EUR: DKK cost / 7.46 = EUR cost
   
2. For 9950X:
   - Same process with 9950X wattage
   - Note difference in annual kWh vs 5700X
```

**Annual Maintenance & Overhead:**
```
1. Thermal Paste Replacement
   - Frequency: Annually (best practice for mining)
   - Cost: ~€15/year per rig
   
2. Dust Cleaning & Filters
   - Frequency: Quarterly
   - Cost: €20–30/year (compressed air, replacement filters)
   
3. Potential Fan Replacement
   - Frequency: Rare in first 3 years
   - Reserve: €0 (or €50/year contingency)
   
4. Pool Fees
   - Already deducted from mining revenue above
   - DO NOT double-count
   
5. Miscellaneous
   - Software updates, monitoring tools: €10–15/year
   
TOTAL OVERHEAD: ~€50–60/year per rig
```

**CRITICAL CHECKPOINT #4:**
Cost Summary:

| Cost Category | 5700X (EUR/year) | 9950X (EUR/year) |
|---------------|-----------------|-----------------|
| Electricity | ? | ? |
| Maintenance | ? | ? |
| Overhead | ? | ? |
| **TOTAL** | **?** | **?** |

---

### **E. TAX TREATMENT (DENMARK 2026)**

Research the following and explain application to mining:

```
1. Self-Employed vs. Corporate Structure
   - RESEARCH: Danish skattemyndighed (tax authority) guidelines
   - FIND: Which structure applies to small mining operation?
   - DOCUMENT: Pros/cons of each (for this analysis, assume self-employed)
   
2. Self-Employed Marginal Tax Rate
   - RESEARCH: 2026 Danish self-employed tax brackets
   - FIND: Statens Skatteadministration official rates
   - COMPONENTS:
     a) Labor market supplementary pension (8%)
     b) Tax rate on business income (approximately 22% + municipal tax 5-8%)
     c) Total effective rate: ~33–35% (research current)
   - VALIDATE: Cross-check multiple sources
   
3. Capital Gains vs. Business Income
   - RESEARCH: Are mining profits taxed as business income or capital gains?
   - FIND: Danish tax law specifics for crypto mining
   - DOCUMENT: How it affects your tax rate
   
4. Depreciation Deduction
   - RESEARCH: Can mining hardware be depreciated in Denmark?
   - FIND: Depreciation schedule (linear, accelerated, etc.)
   - TYPICAL: 22% straight-line or other method
   - CALCULATE: Year 1 depreciation on hardware capital
   - IMPACT: Reduces Year 1 taxable income
   
5. Operating Expenses Deduction
   - Research: Can you deduct electricity, maintenance, etc.?
   - Find: Specific rules for mining expenses
   - Document: What's deductible vs. capitalized
   
6. VAT Considerations
   - Research: Do mining operations need VAT registration?
   - Find: Threshold for VAT registration in Denmark
   - Document: Whether VAT applies to mining revenue
```

**CRITICAL CHECKPOINT #5:**
Tax Impact Summary:

| Tax Component | 5700X (EUR/year) | 9950X (EUR/year) |
|---------------|-----------------|-----------------|
| Gross profit | ? | ? |
| Depreciation (Year 1) | ? | ? |
| Taxable income (Year 1) | ? | ? |
| Tax rate applied | 33% | 33% |
| Tax owed (Year 1) | ? | ? |
| After-tax profit (Year 1) | ? | ? |
| After-tax profit (Year 2+) | ? | ? |

---

## PART 2: SCENARIO MODELING

**Once all variables are researched and validated, create these scenarios:**

### **SCENARIO 1: CPU-ONLY MINING (XMR ONLY, NO MERGED)**

For each CPU (5700X and 9950X):

```
Annual Calculations:
├─ Gross Revenue (XMR only)
├─ Operating Costs (electricity + maintenance)
├─ Gross Profit
├─ Depreciation Deduction
├─ Taxable Income
├─ Tax Owed (Year 1)
├─ After-Tax Profit (Year 1)
└─ After-Tax Profit (Year 2+, steady-state)

Payback Analysis:
├─ Payback Period (years to recover capital)
├─ Annual ROI (year-on-year return %)
├─ 3-year cumulative profit/loss
└─ 5-year cumulative profit/loss

Monthly Cash Flow:
├─ Monthly gross revenue
├─ Monthly costs
├─ Monthly after-tax income (steady-state)
└─ Time to accumulate €1,000 (reinvestment capital)
```

### **SCENARIO 2: MERGED MINING (XMR + AUXILIARY CHAINS)**

For each CPU:

```
Annual Calculations:
├─ Gross Revenue (XMR + merged chains)
├─ Revenue breakdown by chain (show each contributing chain)
├─ Operating Costs (electricity + maintenance)
├─ Gross Profit
├─ [Same tax calculations as Scenario 1]
├─ After-Tax Profit (Year 1)
└─ After-Tax Profit (Year 2+)

Payback Analysis:
├─ Payback Period (years to recover capital)
├─ Annual ROI
├─ 3-year cumulative profit/loss
└─ Comparison vs. CPU-only scenario (€ difference, % improvement)

Monthly Cash Flow:
├─ Monthly after-tax income (steady-state)
└─ Incremental value vs. CPU-only
```

### **SCENARIO 3: 10-YEAR PROJECTION (POST-TAX)**

For each CPU, merged mining:

```
Year-by-Year:
Year 0:   Investment: -€X
Year 1:   Profit: +€Y (with depreciation benefit)
Year 2:   Profit: +€Z (steady-state tax)
Year 3:   Profit: +€Z
...
Year 10:  Profit: +€Z

Cumulative Analysis:
├─ Breakeven year (when cumulative = €0)
├─ Total 10-year profit
├─ Effective 10-year ROI
├─ Per-year average profit (post-breakeven)
└─ Hardware end-of-life consideration (5–7 year typical lifespan)
```

---

## PART 3: RISK ASSESSMENT & SENSITIVITY ANALYSIS

For each scenario, test these sensitivities:

### **Sensitivity 1: Electricity Rate Change**

```
IF electricity rises from 1.6 DKK/kWh to:
├─ 2.0 DKK/kWh (after 24-month reduction ends?)
├─ 2.5 DKK/kWh (higher tax scenario)
└─ 3.0 DKK/kWh (stress case)

IMPACT on profitability:
├─ Annual profit change
├─ Payback period change
└─ Breakeven probability
```

### **Sensitivity 2: XMR Price Change**

```
IF XMR price changes ±20%, ±50%:
├─ Calculate new daily revenue
├─ Recalculate annual profit
├─ New payback timeline
└─ Minimum viable price (below which unprofitable)
```

### **Sensitivity 3: Network Difficulty**

```
Research: Typical difficulty increases over 5 years
├─ Conservative: 30% increase over 5 years
├─ Moderate: 50% increase over 5 years
├─ Aggressive: 100% increase over 5 years

IMPACT:
├─ Revenue reduction (difficulty up = hashrate share down)
├─ New profitability calculations
└─ Breakeven probability
```

### **Sensitivity 4: Hardware Lifespan Risk**

```
Standard: 5–7 year mining lifespan
Optimistic: 8–10 years with excellent maintenance
Pessimistic: 3–4 years if thermal issues occur

QUESTION: What's probability payback achieved before hardware EOL?
├─ 5700X: Payback ? years vs. lifespan 5–7 years
├─ 9950X: Payback ? years vs. lifespan 5–7 years
└─ Risk assessment
```

---

## PART 4: VALIDATION CHECKPOINTS

**Before finalizing, verify:**

```
CHECKPOINT A: Revenue Validation
├─ XMR revenue calculation cross-checked against:
│  ├─ r/MoneroMining recent earnings posts (2026)
│  ├─ Pool statistics (SupportXMR, etc.)
│  └─ Mining calculator websites
└─ Result: ✅ VALID or ❌ FLAG VARIANCE

CHECKPOINT B: Cost Validation
├─ Electricity costs verified against:
│  ├─ User's claimed 1.6 DKK/kWh
│  ├─ Energinet.dk official rates
│  └─ Independent distributor rates (Copenhagen area)
└─ Result: ✅ VALID or ❌ FLAG VARIANCE

CHECKPOINT C: Tax Validation
├─ Tax rates verified against:
│  ├─ Skattemyndighed.dk official 2026 rates
│  ├─ Recent crypto tax guidance (Denmark)
│  └─ Self-employed tax calculator
└─ Result: ✅ VALID or ❌ FLAG VARIANCE

CHECKPOINT D: Profitability Sanity Check
├─ Does annual profit exceed annual costs? ✅ YES / ❌ NO
├─ Is payback within hardware lifespan? ✅ YES / ⚠️ MARGINAL / ❌ NO
├─ Does this align with expected mining economics? ✅ YES / ❌ NO
└─ Result: ✅ CREDIBLE or ❌ INVESTIGATE FURTHER

CHECKPOINT E: Comparison Consistency
├─ Is 9950X clearly superior to 5700X? ✅ YES / ❌ NO
├─ Is the capital difference justified by revenue uplift? ✅ YES / ⚠️ MARGINAL / ❌ NO
└─ Do scenarios make economic sense? ✅ YES / ❌ NO

CRITICAL: If ANY checkpoint fails validation, STOP and investigate before proceeding.
```

---

## PART 5: FINAL OUTPUT STRUCTURE

Present findings in this order:

```
SECTION 1: GROUND TRUTH VARIABLES (documented with sources)
├─ Electricity rate breakdown (1.6 DKK/kWh verification)
├─ Hardware specs & pricing
├─ Mining revenue methodology
├─ Operating costs
└─ Tax treatment

SECTION 2: SCENARIO COMPARISON TABLES
├─ Scenario 1: CPU-only (XMR only)
│  └─ 5700X vs 9950X side-by-side
├─ Scenario 2: Merged mining (XMR + auxiliary)
│  └─ 5700X vs 9950X side-by-side
└─ Scenario 3: 10-year projection (merged mining)
   └─ Year-by-year for each CPU

SECTION 3: RISK ASSESSMENT
├─ Sensitivity analysis (4 key variables)
├─ Breakeven probability analysis
└─ Hardware lifespan vs. payback mismatch risk

SECTION 4: FINAL RECOMMENDATION
├─ Which CPU is economically superior?
├─ What conditions must hold for profitability?
├─ What are key risks?
└─ GO / NO-GO decision for each scenario
```

---

## CRITICAL INSTRUCTIONS FOR RESEARCH

1. **Citation Requirement:** Every numeric value MUST be sourced. If you cannot find a source, say so explicitly and note assumptions.

2. **Variance Flagging:** If your research contradicts the user's 1.6 DKK/kWh claim, flag it immediately at Checkpoint #1 and explain the discrepancy.

3. **No Fabrication:** Do not estimate or "fill in" missing data. If a value is unavailable, state it clearly.

4. **Cross-Validation:** Compare multiple independent sources for critical variables (electricity rates, hashrates, pricing).

5. **Assumptions Transparent:** If you must make an assumption (e.g., "assuming 33% tax rate"), state it and explain the rationale.

6. **Realism Check:** After calculations, ask: "Does this make sense?" If 9950X shows 10× higher profit than 5700X, verify you haven't made an error.

7. **No Projections:** Use current (January 2026) prices/rates. Do NOT project future crypto price changes or difficulty curves unless explicitly modeling sensitivity.

---

## FINAL SANITY CHECK

**Before presenting final recommendation, answer:**

1. ✅ Is 1.6 DKK/kWh electricity rate realistic for Denmark 2026-2027?
2. ✅ Are the hashrate benchmarks credible and recent?
3. ✅ Is the tax treatment accurate for 2026 Denmark?
4. ✅ Does 9950X genuinely outperform 5700X, or is there an error?
5. ✅ What's the minimum breakeven time for each CPU?
6. ✅ What's the biggest risk factor (electricity? difficulty? lifespan?)?
7. ✅ Would I (the researcher) personally deploy this hardware at these economics?

If you cannot confidently answer all seven, flag the gaps before finalizing output.

---

**END OF PROMPT**

Use this as your starting prompt for a new comprehensive unit economics analysis. It should produce consistent, well-sourced results without the errors from the previous chat.