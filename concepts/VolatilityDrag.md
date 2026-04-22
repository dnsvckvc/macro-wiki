---
title: "Volatility Drag"
type: concept
tags: [etf, leverage, derivatives, retail, decay]
sources: [oil-and-retail]
last_updated: 2026-04-21
---

# Volatility Drag

The compounding decay that leveraged and inverse daily-rebalanced ETFs experience when the underlying chops sideways with large daily moves in alternating directions. Even if the underlying finishes flat over a period, a 2x daily-leveraged product finishes down.

## Mechanic
A 2x daily-leveraged ETF (long or inverse) re-sets its exposure every day. If the underlying moves +10% on day 1 and −9.09% on day 2 (round trip to flat), a 2x product is:
- Day 1: `1 + 2×(0.10) = 1.20`
- Day 2: `1.20 × (1 − 2×0.0909) = 1.20 × 0.8182 = 0.982`

→ −1.8% despite the underlying being flat. The larger the daily moves, the larger the drag, compounding geometrically.

## Wiki applications
- **[[SCO]]** — ProShares 2x UltraShort WTI ETF. Per [[oil-and-retail]], retail has pressed ~$1bn into SCO during the Iran/US/Israel war, yet the product has "gone nowhere" despite a significant correction in the flat price. Compounding chop on daily moves of 5–10%+ during the war has eaten the directional bet from the short side.
- Layered effect with **negative carry**: SCO is short a backwardated curve (~$5/mo roll yield against the position in the most backwardated oil market in history), so the drag is structural (curve) *plus* cyclical (vol).
- [[PauloMacro]] cross-references the **2x MSTR levered long/short ETFs of 2024–25** as the same pattern: "the rage" of the retail product complex, simultaneously decayed on both sides.

## Why it matters in the retail-positioning read
The drag turns a "dumb" retail short-oil bet into a quantitatively disastrous one. As [[PauloMacro]] frames it in [[oil-and-retail]]: retail thinks it's "buying the lows" by pressing into a 2x inverse oil vehicle after a crude correction, but the structural decay + negative carry means the only way they can make money is if WTI crashes to zero very quickly — a path that is *specifically* inconsistent with the North-Star/Nash/shut-in scenarios the pros are positioned for.

## Connections
- [[SCO]]
- [[USO]]
- [[PauloMacro]]
- [[oil-and-retail]]
- [[CovidOilCrash2020]] — USO itself suffered structural damage from roll losses during the 2020 contango; the 2026 echo is retail making the mirror-image mistake from the short side
