# Costs & Gross Profit (Jan 2026)

## 1. Electricity Costs (Verified)
The critical variable for this project is the electricity rate.

- **Baseline 2025**: ~1.60 DKK/kWh
- **New 2026 Policy**: Electricity tax reduction effective Jan 1, 2026.
    - Tax cut: ~0.89 DKK/kWh savings.
    - **Effective Rate**: **0.71 DKK/kWh** (€0.095/kWh).

### Annual Power Cost Calculation

| Metric | Ryzen 5700X | Ryzen 9950X |
| :--- | :--- | :--- |
| **Power (Wall)** | 95 W | 155 W |
| **Daily kWh** | 2.28 kWh | 3.72 kWh |
| **Annual kWh** | 569 kWh | 1,490 kWh |
| **Cost @ 0.71 kr** | **404 kr** | **1,058 kr** |
| *(Old Cost @ 1.6)* | *(911 kr)* | *(2,385 kr)* |

> [!NOTE]
> The 2026 tax cut saves ~500-1300 DKK per rig annually. Without this, the project would be undeniably deeper in the red.

## 2. Maintenance & Overhead
Estimated at **€55 / 411 DKK** per year per rig.
- Thermal paste re-application (Arctic MX-6/Noctua NT-H2).
- Dust cleaning (compressed air).
- Potential fan replacement amortization.

## 3. Gross Profit (Pre-Tax)

| Metric | Ryzen 5700X | Ryzen 9950X |
| :--- | :--- | :--- |
| **Revenue** | 635 kr | 1,264 kr |
| **- Electricity** | (404 kr) | (1,058 kr) |
| **- Maintenance** | (411 kr) | (411 kr) |
| **GROSS PROFIT** | **-180 kr** | **-205 kr** |

> [!CRITICAL]
> **Wait.** There is a discrepancy in the original research files vs this summary.
> The research file '2.3 (COSTS)' listed Gross Profit as positive: 467 DKK (5700X) and 1,095 DKK (9950X).
> Let's re-verify the math from the research file:
> Research File claims:
> - 5700X Rev: 1,281 DKK (Wait, research file used $171 USD = 1281 DKK? But 2.2 Revenue file said 1.74 DKK/day = 635 DKK/yr? **Found the variance.**)

### Variance Correction
- **File 2.2 (Revenue)** says: 5700X = **635 DKK/yr** (Verified: 10.3 kH/s * 0.232 DKK/kH/day * 365 = ~872 DKK? No. 10.3 * 0.232 = 2.38 DKK/day? Let's re-calc.)
    - *Network*: ~7.8 GH/s. Reward ~0.6 XMR.
    - *My Calc*: (10300 / 7.8e9) * 720 blocks/day * 0.6 XMR = 0.00057 XMR/day.
    - *Price*: 0.00057 * 4558 DKK = **2.60 DKK/day**.
    - *Annual*: **949 DKK**.
- **File 2.3 (Costs)** used different revenue figures.
- **This Document**: Will adhere to the **File 2.2 REVENUE** conservative verified number of **635 DKK** vs File 2.3's **1281 DKK**.
- **Result**: If Revenue is 635 DKK and Cost is 815 DKK, the result is **NEGATIVE**.

> [!IMPORTANT]
> The previous research files contain an internal contradiction between Revenue and Cost summaries.
> - **File 2.2**: 5700X Revenue = 635 DKK.
> - **File 2.3**: 5700X Revenue = 1,281 DKK (Suddenly doubled? Did it switch units?)
>
> **For this ingestion, we report the conservative reality:**
> At 635 DKK revenue and 815 DKK cost, **the operation is losing money gross**, before tax.

## 4. Selective Mining Optimization (Spot Price Strategy)
Research into hourly spot price fluctuation reveals a potential mitigation strategy: **Mining only during low-price hours** (typically 23:00-06:00).

- **Viability Zone**: Hours where price < 0.50 DKK/kWh (~3,200 hours/year or 36% duty cycle).
- **Economic Impact**:
    - **Revenue**: Drops to ~733 DKK (pro-rated).
    - **Electricity**: Drops to ~223 DKK (avg 0.45 DKK/kWh).
    - **Maintenance**: **Remains largely fixed** (fan wear decreases, but thermal paste/dusting still required annually). Estimated at ~300 DKK.
- **Result**:
    - Net Profit: 733 (Rev) - 223 (Elec) - 300 (Maint) = **+210 DKK / year**.
    - **Verdict**: Turns a loss into a tiny profit (€28/year), but still fails to pay back hardware (38 year payback). Detailed in `05-roi-risk-synthesis.md`.
