---
title: "Liquidity Mechanics (TGA / RRP / Bank Reserves)"
type: concept
tags: [liquidity, fed, treasury, tga, rrp, reserves, market-structure]
sources: [liquidity-drains, liquidity-drains-redux, the-north-star-vs-liquidity, could-fed-liquidity-plunge-by-half]
last_updated: 2026-04-12
---

# Liquidity Mechanics (TGA / RRP / Bank Reserves)

[[PauloMacro]]'s framework for tracking the "beating heart" of US system liquidity via three interrelated variables on the Fed's balance sheet. **Origin document:** [[liquidity-drains]] (March 2024), which provides the full mechanics primer and Yellen's TGA-smoothing playbook. Applied in [[the-north-star-vs-liquidity]] (April 2026) to explain the risk-asset bounce under Bessent's TGA management — the same mechanics, different Treasury Secretary.

## The three variables
1. **Fed balance sheet assets** — when rising (QE, RMP), bank reserves grow → liquidity up.
2. **Fed Reverse Repo (RRP)** — a liability; when declining, liquidity enters the banking system → liquidity up. (Drained to essentially zero by early 2026.)
3. **Treasury General Account (TGA)** — a liability; the Treasury's checking account. When spending exceeds issuance (TGA draws down), cash flows into the banking system → liquidity up. When tax receipts or new issuance exceeds spending (TGA rebuilds), liquidity drains.

**Rule of thumb:** assets up OR liabilities down → liquidity up → risk assets bid.

**Core identity (from [[liquidity-drains]] appendix):** Liquidity ≈ Fed Balance Sheet (SOMA) − TGA − RRP, assuming bank reserves stay flat. Only two things truly suck liquidity: raising the TGA (Treasury issues debt but doesn't spend) or QT. The fiscal deficit itself is not a liquidity drain if Treasury spends immediately — the money goes right back to bank accounts.

## Bessent's TGA: a two-way tool (drain vs inject)
The key insight across both the [[liquidity-drains-redux]] (August 2025) and [[the-north-star-vs-liquidity]] (April 2026) is that the Treasury Secretary's TGA management is **a two-directional mechanism** using the same plumbing:
- **2025 (drain):** Bessent rebuilds the TGA by ~$250bn. With RRP at $78bn (zero buffer), the drain comes from bank reserves. Overnight GC repo ticks toward the top of the Fed corridor. Crypto — the most liquidity-sensitive asset class — falls first. This triggers the 4Q25 quant quakes and the [[RollingVARShock]].
- **2026 (inject):** Bessent draws the TGA *down* by $200bn+ ahead of April 15 tax receipts, injecting liquidity. Combined with Fed RMP, bank reserves rise $100bn+ in two weeks. This fuels the post-ceasefire risk rally that confounds bears.

## 2025–2026 liquidity cycle
- **3Q 2025:** Fed QT + TGA rebuild drained bank reserves by ~$600bn. Quant quakes in July and September. Short-term rates breached the Fed Funds corridor in 4Q25 (echoing September 2019 repo problems).
- **December 2025:** Fed abandoned QT and initiated the **RMP** (Reserve Management Purchase program) to replenish reserves.
- **Late March–early April 2026:** [[ScottBessent]] held back debt issuance ahead of April 15 tax receipts, drawing the TGA down ~$300bn from late 2025 (~$200bn since end of March alone). Combined with RMP, bank reserves rose ~$250bn since late last year ($100bn+ in just 2 weeks).
- This liquidity injection collided with a hedge-fund positioning washout (largest weekly ETF short-covering in a decade) to produce the "ceasefire" risk rally.

## Why it's short-term
- **April 15 tax payments** will flow into the TGA, reversing the liquidity tailwind. Only the relatively small RMP remains as a source of injection.
- Paulo: *"the market tends to react immediately on the upside to fresh liquidity but needs time to roll over on declining liquidity — reacts like an elevator, drops by the stairs until it trips and falls."*
- This sets up the traditional "Sell in May" seasonal.

## Role in the wiki
Liquidity mechanics explain *why* the market bounced despite the [[NorthStar]] (Nash / Iran's strategy is unchanged) and the physical-world "Can't Print Molecules" reality. The bounce is real and mechanical, not a sign that the thesis is wrong — it just sets up a bigger snap-back when the liquidity tailwind fades and hedges have been stripped.

## Howell's elegant formulation (per [[could-fed-liquidity-plunge-by-half]])
**Liquidity = assets / duration.** Two ways to increase liquidity: grow the asset pool (same duration) or reduce average duration (same asset pool). The Fed can only do the latter (maturity transformation); the Treasury can do *both* (increase total debt + shift from notes to bills). This is why the coordination between Fed and Treasury is critical, and why Paulo's [[ScottBessent]] TGA observations are so load-bearing: Bessent's issuance timing *is* the coordination mechanism.

**"Treasury QE" replacing "Fed QE":** The policy shift where Treasury bills replace Fed reserves as the primary liquidity instrument. Satisfies the administration's desire to reduce the Fed's influence — but requires explicit coordination that "rarely exists in practice."

**Inelasticity at low reserves:** At lower reserve levels, the demand curve becomes more inelastic → small demand/supply shifts cause big rate swings. This is exactly what Paulo documented in [[liquidity-drains-redux]] (repo rates ticking toward the corridor ceiling) and what the [[StephenMiran]]/Fed paper ignores.

## Relationship to the [[GlobalLiquidityCycle]] ([[MichaelHowell]])
Paulo's TGA/RRP/bank-reserves framework is the **US micro-plumbing** layer. [[MichaelHowell]]'s ~65-month Global Liquidity Cycle ([[the-liquidity-tide-goes-out]]) is the **macro overlay**:
- Howell explains *why* the broad tide is going out (the cycle peaked Q4 2025 / early 2026; central banks outside the US — ECB, BoE, BoJ — continue balance-sheet shrinkage; trillions in debt rollovers absorbing liquidity).
- Paulo explains the *specific US mechanics* that create short-term counter-trend injections (Bessent TGA drawdown, Fed RMP) within that broader downswing.
- Howell's key distinction — **level vs. momentum** — means the real economy can keep growing ($188T absolute liquidity) while risk-asset rallies fade (negative momentum). This is the macro frame for why "Can't Print Molecules" coexists with a still-functional economy.

## Connections
- [[PauloMacro]]
- [[ScottBessent]]
- [[NorthStar]]
- [[Degrossing]]
- [[JeromePowell]]
- [[GlobalLiquidityCycle]]
- [[MichaelHowell]]
- [[StephenMiran]]
