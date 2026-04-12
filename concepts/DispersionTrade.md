---
title: "Dispersion Trade"
type: concept
tags: [options, volatility, correlation, hedge-fund, market-structure]
sources: [making-macro-great-again-quick-updates, the-anatomy-of-a-crash]
last_updated: 2026-04-12
---

# Dispersion Trade

A relative-value options strategy that harvests the spread between **implied correlation** and **realized correlation**. Mechanically:

- **Long** single-stock volatility (buy options on individual names).
- **Short** index volatility (sell options on SPX / NDX).

The trade pays off when individual stocks move around a lot on their own schedules (realized single-stock vol is high) while the index is relatively quiet because the individual moves cancel out (realized index vol is low). In other words, it is short implied correlation.

## Why [[PauloMacro]] calls it his "single biggest concern" ([[the-anatomy-of-a-crash]])
As of mid-March 2026, **rising correlation** is eating the long leg:
- 1-month implied correlation jacked to multi-year highs; 1m–3m spread exploded.
- Stocks start moving *together*, which kills the vol-harvesting edge on the long book.
- Paulo's direct evidence: on a trade to buy AirBNB June puts, his quote was **gapped *above*** his bid for the first time ever — implied vol jumped 40 → 55+, and the options quote stayed wide and shifted range. Confirming John Flood's (GS) warning that single-stock liquidity is much worse than screens indicate.
- When the long leg starts losing money persistently, the trade must **degross**, which means buying index vol to cover the short leg.
- That buying **releases index vol**, and the feedback loop accelerates: index vol rises → realized index vol rises → more correlation → more loss → more degrossing. "S&P starts dropping 1.5–3% per day."

## Monitoring data point (per [[making-macro-great-again-quick-updates]], 12 March 2026)
- 1-month implied correlation has jacked up to **Liberation Day / SVB crisis levels**; the 1m–3m correlation spread has blown through multi-year highs.
- However, VIX has only reached "Bear Stearns VIX 30" fear — **not "The Fear"** (Liberation Day / Yenmageddon levels).
- This divergence (correlation screaming, VIX still muted) is exactly the setup Paulo predicts will break: correlation has room to keep rising, and once it does, the Dispersion long book buckles → degrossing → index vol release → The Fear.
- Paulo: *"Are the Dispersion Bros finally about to lose control?"*
- Investors are sitting on near-dated puts that aren't paying off — they've bought hedges but haven't sold. The transition from hedging to [[Degrossing]] has not happened yet, which is why VIX lags.

## Why this is the trigger
The dispersion trade is the one strategy that has *not* yet felt pain in the [[RollingVARShock]] sequence. Once it blows, there is no remaining volatility-suppressing mechanism in the book.

## Connections
- [[PauloMacro]]
- [[RollingVARShock]]
- [[AnatomyOfACrash]]
- [[TurduckenOfMarketRisks]]
- [[Degrossing]]
