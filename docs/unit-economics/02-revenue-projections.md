# Revenue Projections (Jan 2026)

**Protocol**: Monero (RandomX)
**Pool**: SupportXMR (PPLNS)

## 1. Market Assumptions
- **XMR Price**: €610.72 (~4,558 DKK)
- **Network Difficulty**: ~300 GH (Stable/Slow growth assumption for baseline)
- **Block Reward**: 0.6 XMR (Tail emission)

## 2. Daily Earnings (XMR Only)

| Metric | Ryzen 5700X | Ryzen 9950X |
| :--- | :--- | :--- |
| **Hashrate** | 10.30 kH/s | 20.40 kH/s |
| **Daily Rev (EUR)** | €0.233 | €0.464 |
| **Daily Rev (DKK)** | **1.74 kr** | **3.47 kr** |
| **Annual Rev (DKK)** | **635 kr** | **1,264 kr** |

> [!WARNING]
> These revenue figures are **gross**. They do not include electricity. At 1.74-3.47 kr/day, the revenue stream is extremely thin.

## 3. Merged Mining Analysis (Tari / XTM)
**Verdict: NO-GO for Home Mining**

We investigated merged mining Tari (XTM) alongside Monero.
- **Status**: Active (P2Pool v4.0+).
- **Reality**: Tari mining is currently effectively **solo-only** for block rewards.
- **Probability**: A home miner with 10-20 kH/s faces a time-to-find-block of **70–468 days**.
- **Expected Uplift**: Even averaged perfectly, uplift is <5% (~0.07-0.15 DKK/day).
- **Recommendation**: Ignore merged mining complexity for this scale. Stick to SupportXMR pool for consistent XMR payouts.
