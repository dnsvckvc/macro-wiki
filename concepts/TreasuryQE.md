---
title: "Treasury QE"
type: concept
tags: [treasury, fed, qe, bills, buybacks, howell, bessent]
sources: [treasury-qe-warsh-fed-eclipsed, crypto-gold-pboc-vs-fed, could-fed-liquidity-plunge-by-half]
last_updated: 2026-04-27
---

# Treasury QE

The set of operational tools the **US Treasury** uses to inject liquidity *as if* doing QE — but without the Fed expanding its balance sheet. The operational core of the [[StealthAccord]]. Defined explicitly by [[MichaelHowell]] in [[treasury-qe-warsh-fed-eclipsed]] (25 April 2026).

## The two pillars

### Pillar 1: Skew issuance toward bills

The Treasury currently issues a higher-than-normal share of debt as **Treasury bills** (short-term, <1 year): **22.2% of total debt outstanding.**

Why bills create liquidity:
- Banks create liquidity through *maturity transformation* (borrow short, lend long), but only the *public* sector creates **net credit** — assets for the private sector with no matching liability.
- The shorter the duration of government liabilities, the larger the liquidity boost (the bill is *almost cash* for the holder).
- *"Banks buy bills, M2 grows, and the economy gets a stimulus — without the Fed lifting a hand."*

This is **stealth monetization**: M2 grows, real-economy credit conditions ease, no formal QE announcement required.

### Pillar 2: Volatility-targeting buybacks

The Treasury buys less-liquid **off-the-run** bonds and replaces them with new **on-the-run** securities. Effects:
- Lifts market liquidity in the off-the-run segment (the largest part of the market).
- Compresses the [[MOVEIndex]].
- Each 10-point rise in MOVE → ~**$30 billion** increase in buyback volumes (empirical Howell rule).

These are operationally distinct from old-style "twist" operations because the trigger is **bond volatility** (MOVE), not curve shape or term structure.

## Why Treasury QE is more powerful than Fed QE in the current regime

Per Howell's [[CollateralMultiplier]] framework: each **10-point fall in MOVE → ~$3 trillion (1.5%)** of additional Global Liquidity. Treasury QE acts directly on MOVE and therefore has a **~100× leverage ratio** between buyback volume and resulting Global Liquidity creation:

```
$30bn buyback per 10pt MOVE rise → 10pt MOVE fall later → $3T Global Liquidity expansion
```

Howell's chart in [[treasury-qe-warsh-fed-eclipsed]] shows Fed QE (red and orange — balance-sheet expansion + compositional changes / "Not QE, QE") **declining** through 2026 while Treasury QE (buybacks + bill issuance) **rises strongly**.

> *"The US Treasury has replaced the Fed as the marginal driver of US and Global Liquidity."*

## Why this is different from the 1951–1953 era

- 1951–1953: Fed and Treasury were *formally* coordinated (the prior Accord explicitly capped rates to support war-debt issuance).
- 2025/26: the merger is *informal*. Neither party admits to monetizing debt; the data shows it is happening.

> *"Neither party, Fed or US Treasury, admits to monetizing debt. But these policies facilitate and encourage precisely that."*

## Wiki cross-references

This concept consolidates several scattered observations:
- The phrase "Treasury QE" first appeared in the wiki via [[could-fed-liquidity-plunge-by-half]] (1 April 2026): *"the policy shift where Treasury bills replace Fed reserves as the primary liquidity instrument."*
- [[ScottBessent]]'s **$15B single-day Treasury buyback** (largest in history, executed after three ugly UST auctions) per [[macrovoices-528-luke-gromen]] is the most visible single Treasury-QE intervention to date.
- [[LukeGromen]]'s **4.4% UST yield bogey** is a Treasury-QE *trigger threshold*: every break above 4.4% causes Bessent intervention.
- [[PauloMacro]]'s [[the-north-star-vs-liquidity]] documented the **$300bn TGA drawdown** (December 2025 → April 2026) which is the *liability-side* mirror of Treasury QE — Bessent injecting liquidity by holding back issuance ahead of April 15 tax receipts.

Together these form Howell's "Treasury QE" as it has actually been operationalized through 2025–2026.

## Risks (per [[treasury-qe-warsh-fed-eclipsed]])

- **Moral hazard:** markets expect buybacks → larger leveraged [[BasisTrade]] positions → bigger eventual unwind.
- **Collateral fragility:** if MOVE spikes *despite* buybacks (e.g., geopolitical shock), the [[CollateralMultiplier]] collapses and Global Liquidity contracts mechanically. March 2020 COVID is the precedent.

## Connections
- [[StealthAccord]] — the regime under which Treasury QE operates.
- [[CollateralMultiplier]] — the quantitative mechanism that makes Treasury QE more powerful than Fed QE.
- [[MOVEIndex]] — the joint dial.
- [[ScottBessent]] — the operator.
- [[KevinWarsh]] — the constrained successor.
- [[ReserveManagementPurchases]] — Fed-side coordination dial; now subordinated to Treasury-side.
- [[BasisTrade]] — the leveraged-trade Pillar that benefits from suppressed MOVE.
- [[LukeGromen]] — the 4.4% yield bogey + $15B buyback observation.
- [[PauloMacro]] — TGA-drawdown observations are the liability-side mirror.
- [[LiquidityMechanics]] — Paulo's framework that this piece subsumes.
