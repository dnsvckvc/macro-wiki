---
title: "MOVE Index"
type: concept
tags: [bond-volatility, treasury, basis-trade, liquidity, bassman]
sources: [crypto-gold-pboc-vs-fed, vix-inversion-buying-bonds-japan-jpm-option-whale, bond-markets-point-the-way, treasury-qe-warsh-fed-eclipsed]
last_updated: 2026-04-27
---

# MOVE Index

The **Treasury bond volatility index** — the fixed-income equivalent of the VIX. Created by [[HarleyBassman]] at Merrill Lynch in 1988. Tracks the implied volatility of US Treasury options across the curve.

## Why it matters in the wiki

[[MichaelHowell]]'s 27 April 2026 piece ([[crypto-gold-pboc-vs-fed]]) elevates the MOVE Index to **the third engine of Global Liquidity**, alongside the US Fed and the [[PBOC]]:

> *"In our collateral-based World, low bond volatility is crucial. It not only supports the on-going [hedge fund] [[BasisTrade]], but it is a crucial pillar in Global Liquidity creation."*

## The two quantitative rules — Howell's MOVE arithmetic

Howell's framework gives **two** quantitative rules linking MOVE to liquidity:

| Rule | Direction | Magnitude | Source |
|---|---|---|---|
| **Buyback response** | MOVE rises 10pts | Treasury buybacks rise ~$30bn | [[crypto-gold-pboc-vs-fed]] (27 Apr) |
| **Liquidity creation via [[CollateralMultiplier]]** | MOVE falls 10pts | Global Liquidity rises ~$3T (1.5%) | [[treasury-qe-warsh-fed-eclipsed]] (25 Apr) |

These compose into ~100× leverage between Treasury buyback dollars and resulting Global Liquidity creation:
```
$30bn buyback → 10pt MOVE compression → $3T Global Liquidity expansion
```

This is *why* MOVE has become the master dial of Howell's [[StealthAccord]]: it is not just a Fed-policy-stress indicator; it is the *quantitative pivot* through which Treasury operations create stealth liquidity, regardless of where the Fed sets rates.

The mechanism: when bond vol rises, Treasury market structure deteriorates ([[BasisTrade]] participants can't fund positions, dealers reduce inventory, market depth thins) → Treasury responds with buybacks to absorb supply and stabilize the curve → MOVE compresses → [[CollateralMultiplier]] expands → Global Liquidity creation occurs *automatically* via the dealer/repo system.

This is the formal coordination point that makes [[TreasuryQE]] operationally distinct from monetary policy: the [[ScottBessent]]-led Treasury actively manages bond volatility via discretionary buyback timing, which then triggers the multiplier mechanism.

## Howell's threshold

> *"We view anything below 80 as a stimulus to Global Liquidity."*

- MOVE peaked at **115 on March 26, 2026** (in the second half of the war-induced sell-off).
- Closed the week of 25 April at **67** — well below the 80 stimulative threshold.
- The fall from 115 → 67 = **~14 × $30bn ≈ $420bn equivalent of Treasury-buyback-style liquidity** restored.

## The four-signal watchlist (Howell)

The MOVE Index is one of four indicators on Howell's *"warnings of upcoming trouble"* dashboard:

1. SOFR spreads (must stay near zero)
2. **MOVE Index** (stay around 80)
3. 10-2 yield curve (avoid bearish flattening)
4. Gold + Crypto prices (do not break lower)

A break above 80 in MOVE = the third engine of Global Liquidity is failing.

## Cross-author references

- [[KevinMuir]] uses MOVE as a Fed-policy-stress indicator alongside the [[VIX7v2Spread]]. His long fixed-income trade (long whole curve, 2s/5s overweight, [[HarleyBassman]]'s **TUA ETF**) *benefits* from MOVE compression. ([[vix-inversion-buying-bonds-japan-jpm-option-whale]])
- [[PauloMacro]] flags rising MOVE as one component of the [[TurduckenOfMarketRisks]] regime, with **credit vol leading MOVE** as a "first this cycle" signal in [[the-anatomy-of-a-crash]].
- Howell in [[bond-markets-point-the-way]]: the Iran shock added ~20pts to MOVE alongside oil + DXY = ~20% hit to Global Liquidity if sustained.

## Connections
- [[HarleyBassman]] — creator of the index; TUA ETF designer.
- [[BasisTrade]] — what low MOVE protects.
- [[GlobalLiquidityCycle]] — MOVE is the third-engine dial.
- [[LiquidityMechanics]] — Treasury buyback responses to MOVE are the Treasury-side mechanic.
- [[ScottBessent]] — operator of the buyback mechanism.
- [[ReserveManagementPurchases]] — the Fed-side counterpart.
- [[VIX7v2Spread]] — Muir's equity-vol equivalent.
- [[StealthAccord]] — the regime in which MOVE has become the master dial.
- [[TreasuryQE]] — the Treasury-side mechanism MOVE coordinates.
- [[CollateralMultiplier]] — the quantitative mechanism through which MOVE translates into Global Liquidity.
