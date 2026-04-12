---
title: "Charm (Options Greek)"
type: concept
tags: [options, greeks, dealer-gamma, market-structure]
sources: [vix-inversion-buying-bonds-japan-jpm-option-whale]
last_updated: 2026-04-12
---

# Charm

A second-order options greek: **the change in delta from the passage of time**. Also known as delta decay. Tells you how an option's delta drifts purely as time approaches expiry, holding everything else constant.

## Why it matters for dealer hedging
For a dealer who is short a put and short futures against it (delta-hedged), charm determines whether the passage of time forces them to *buy* or *sell* more futures to stay hedged.

- **Spot above the put strike:** as time passes, the put becomes less likely to finish in the money, its delta drifts toward zero, and dealers must *buy back* futures to keep the hedge correct. Positive charm (from their perspective) — a natural dampener.
- **Spot below the put strike:** the put is ITM; as time passes, its delta drifts toward −1 (full hedge needed), and dealers must *sell more* futures. **Negative charm** — time itself adds to the selling pressure, all else equal.

## Application in the wiki
[[KevinMuir]] in [[vix-inversion-buying-bonds-japan-jpm-option-whale]] walks through this mechanic for the [[JPMCollarTrade]] in the unusual regime where spot had fallen *through* the 6475 long-put strike. As a result, on top of the usual short-gamma delta-hedging cascade, dealers were also subject to negative charm — time alone was creating additional delta selling. This is the rare and uncomfortable "three-greek" configuration (gamma + vanna + charm all pushing the same way) that makes a trade like the JPM whale a "HUGE SOURCE OF INSTABILITY."

## Connections
- [[JPMCollarTrade]]
- [[KevinMuir]]
- [[TurduckenOfMarketRisks]]
