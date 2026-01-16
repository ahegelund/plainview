# Research Methodology & Framework

This documentation set establishes the unit economics for the Plainview mining rig project. It is consistent with the "Plainview 2.1-2.5" research series conducted in January 2026.

## Research Objectives
Conduct a comprehensive, self-validating unit economics analysis for CPU mining two Ryzen configurations (5700X vs 9950X) in Denmark with verified electricity pricing (2026 tax-cut adjusted).

## Methodology
The research follows a strict 5-stage process with validation checkpoints to minimize hallucination and error.

### 1. Ground Truth Variables
- **Electricity Data**: Validated against Danish 2026 tax reforms (Energinet.dk, Skatteministeriet).
- **Hardware Pricing**: Sourced from German/EU retailers (Mindfactory, Caseking) with 25% VAT consideration.
- **Currency**: All final modeling in DKK, using verified EUR/DKK exchange rates.

### 2. Validation Checkpoints
- **Revenue Check**: Cross-referenced with mining pools (SupportXMR) and real-time network difficulty.
- **Cost Check**: Validated power wall-draw (not just TDP) against third-party reviews.
- **Realism Check**: "Does this payback period make sense?" (12+ years confirmed as realistic for this tariff).

## Source Files
The following original research prompts and outputs were used to generate this data:
- `Mining_Unit_Economics_Research_Prompt.md` (Framework)
- `Prompt_Usage_Guide.md` (Process)
- `2.1__CRITICAL INSTR.md` (Specs)
- `2.2 (REVENUE)__CRIT.md` (Revenue)
- `2.3 (COSTS)__CRITIC.md` (Costs)
- `2.4 (TAX & NET.md` (Tax)
- `2.5 (UNIT ECONOMICS.md` (ROI)
