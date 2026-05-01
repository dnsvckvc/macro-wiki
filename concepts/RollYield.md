---
title: "Roll Yield"
type: concept
tags: [commodities, futures, term-structure, backwardation, contango, etf, passive-investing]
sources: [macrovoices-529-ole-hansen, oilgroundup-adi-imsirovic, oil-and-retail]
last_updated: 2026-04-23
---

# Roll Yield

The **return component a passive long futures investor earns or loses from rolling expiring contracts** into the next month, separate from the spot-price move. Positive in backwardation, negative in contango.

Mechanics ([[OleHansen]] in [[macrovoices-529-ole-hansen]]): ETFs and swaps that give clients commodity exposure must continuously roll futures positions. In **backwardation**, the expiring contract is more expensive than the next contract — sell high, buy low → **positive roll yield**. In **contango**, sell low, buy high → **negative roll yield** ([[VolatilityDrag]] is the daily-rebalanced ETF version of this).

## The wiki's canonical case study — Hansen's slide 4

Bloomberg Spot Index vs. Bloomberg Total Return Index, in two consecutive 5-year cycles:

| Period | Curve regime | Spot Index | Total Return Index | Difference |
|---|---|---|---|---|
| 2016–2021 | mostly contango | +52% | +14% | **−38pp drag** |
| 2021–2026 | mostly backwardation | +57% | +83% | **+26pp tailwind** |

Hansen: *"That massive difference is basically because we had a period, a number of years, where most markets were trading contango. Fast forward to the last five years from 2021 to 2026… If you look at the total return, you're actually up 83%. That is a massive difference in the performance of your investment."*

## Current scale (April 2026)

- Brent forward curve: ~**$12.50 backwardation** June → December.
- Hansen: *"If you bought the December contract and waited for it to come to expiry in six months, you'd be making 15% on that investment in six months. So what does that annualize to? A whole lot."*
- Roll mechanics example: rolling June ($95) into July ($90) → +$5 instant carry if spot stays at $95.

## Why it matters

- **Passive long is now an actually rewarding trade.** For most of 2016–2021 the curve was eating returns; even directional bulls were dragged down by negative roll. Now, even a sideways spot tape generates meaningful returns.
- **Why "natural gas is such a dog"** for long-only investors (Hansen): seasonal contango through summer storage builds means the roll relentlessly destroys passive-long capital.
- **Producer hedging brake** ([[OleHansen]]): when the curve is steeply backward, hedging 3–6 months out captures *much lower* prices — disincentivizing new drilling. Explains why six weeks of war + $90+ crude has produced **zero new US rigs and zero new US barrels**.

## Connections

- **[[BrentComplex]]** — the term-structure section.
- **[[TheoryOfStorage]]** — the academic foundation for which curve shape is "natural."
- **[[VolatilityDrag]]** — the daily-rebalanced-leveraged-ETF cousin (e.g. [[SCO]]) that compounds *against* the holder.
- **[[BrickAndMortarTrade]]** — the physical-market scarcity that creates extreme front-end backwardation.
- **[[PrecautionaryDemand]]** — Johnston's mechanism for the front-end pricing pressure that sustains positive roll yield.

## Cross-sector applicability (Hansen)

| Commodity | Curve as of April 2026 |
|---|---|
| Brent / WTI | Steep backwardation ($12+ June→Dec) |
| Soybean oil | Backwardated (biofuel link) |
| Coffee | Decent backwardation |
| Wheat / corn | Still ~10% one-year contango |
| Natural gas | Seasonal contango |

For agriculture, anything below 5% (the one-year USD funding cost) signals a tightening market.
