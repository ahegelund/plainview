# Plainview Rig Project

**Status:** NO-GO (Economic Unviability)
**Location:** Denmark (Copenhagen)
**Era:** 2026 (Post-Tax Reform)

## Executive Summary
This repository documents the research and unit economics for a proposed home CPU mining operation ("Plainview"). 

**Conclusion:** Despite a significant 2026 Danish electricity tax reduction (from 1.6 to 0.71 DKK/kWh), the operation remains economically unviable. The projected payback period exceeds **30 years**, far outlasting hardware lifespan.

## Unit Economics (2026 Verified Figures)

The following figures use verified conservative estimates for Monero (RandomX) mining.

### 1. Capital Investment (CapEx)
| Rig Configuration | CPU Price | Platform Cost | **Total CapEx** |
| :--- | :--- | :--- | :--- |
| **Ryzen 7 5700X** | ~€172 | ~€413 | **4,369 kr** (€585) |
| **Ryzen 9 9950X** | ~€513 | ~€560 | **8,015 kr** (€1,073) |

### 2. Annual Operating Metrics (OpEx vs Revenue)
*Electricity Rate: 0.71 DKK/kWh (effective 2026)*

| Metric | Ryzen 5700X | Ryzen 9950X |
| :--- | :--- | :--- |
| **Hashrate** | 10.3 kH/s | 20.4 kH/s |
| **Power (Wall)** | 95 W | 155 W |
| **Annual Revenue*** | **~635 kr** | **~1,264 kr** |
| **Annual Electricity** | -404 kr | -1,058 kr |
| **Maintenance** | -411 kr | -411 kr |
| **Net Profit (Annual)** | **-180 kr (LOSS)** | **-205 kr (LOSS)** |

*\*Revenue based on verified SupportXMR pool data (Jan 2026).*

### 3. Investment Analysis
- **Payback Period**: **Infinite** (Operational Loss)
- **Optimized Strategy (Selective Mining)**: Mining only during cheap overnight hours (<0.50 DKK/kWh) yields a tiny annual profit of ~210 kr.
    - Resulting Payback: **38 Years** (Still unviable).
- **Risk**: If the 2026 electricity tax cut expires in 2028, operating costs double, guaranteeing heavy losses.

## Critical Discrepancy Note
Initial research files contained a discrepancy where revenue was artificially doubled in the Cost analysis. This repository corrects that error. **We rely on the verified revenue of ~0.03 EUR/kH/day.**

## Documentation
Full detailed breakdown available in `docs/unit-economics/`:
- [Hardware Specs](docs/unit-economics/01-hardware-specs.md)
- [Revenue Projections](docs/unit-economics/02-revenue-projections.md)
- [Costs Analysis](docs/unit-economics/03-costs-and-gross-profit.md)
- [Tax Framework](docs/unit-economics/04-tax-framework.md)
- [ROI Synthesis](docs/unit-economics/05-roi-risk-synthesis.md)
