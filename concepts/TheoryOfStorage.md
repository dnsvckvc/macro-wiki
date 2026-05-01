---
title: "Theory of Storage"
type: concept
tags: [oil, commodities, term-structure, microstructure, academic]
sources: [oilgroundup-adi-imsirovic, macrovoices-529-ole-hansen]
last_updated: 2026-04-23
---

# Theory of Storage

The academic foundation for understanding why commodity futures curves take the shapes they do. Originally developed for agricultural commodities (wheat, corn) in the early 20th century and central to modern oil-market term-structure analysis. References "convenience yield" — the implicit return from holding physical inventory rather than financial claims.

## Two rival framings

### Classical theory of storage (Imsirovic's view)
- **Contango is the natural state.** Backwardation is the "wrong way round" — *backward* — and requires a scarcity explanation.
- In a well-supplied market, the curve must pay for storage (tank rental, insurance, capital, losses). That payment = contango.
- Backwardation arises only when the physical market is tight enough that the opportunity cost of *not* delivering now exceeds the cost of holding inventory.
- Per [[AdiImsirovic]] in [[oilgroundup-adi-imsirovic]]: *"contango is a natural state of the market. Backwardation is as the word says, backward."*

### Keynesian normal-backwardation (Bouchouev's view)
- **Backwardation is natural state** because producers hedge their forward production more aggressively than end-users hedge their forward consumption.
- Systematic long-dated producer selling pressure drives futures prices below expected spot → backwardation = equilibrium.
- Rory's gloss: *"A paper-barrel SD view."*
- Attributed by Imsirovic (a "friend and great teacher") to [[IlyaBouchouev]].

Both views are *internally consistent* — they disagree about which effect dominates. The oil-market literature has never definitively settled the debate.

## Why the debate matters for the April 2026 crisis
- If contango is natural (Imsirovic), then $15-$30 backwardation is an extreme statistical event requiring a scarcity-driven explanation → panic.
- If backwardation is natural (Bouchouev), then $15-$30 backwardation is a large deviation from an already-backward baseline → still panic, but the counterfactual is different.
- Either way, the current print is historic. Both views end at "this is a panic-driven scarcity signal, not a regime change in term-structure behavior."

## The portfolio-management consequence ([[macrovoices-529-ole-hansen]])
Whatever the academic framing, [[OleHansen]] makes the **practical** case in [[macrovoices-529-ole-hansen]]: term-structure shape *is* the driver of passive-investor returns over multi-year horizons. The 2016–2021 contango era cost Bloomberg Total Return Index ~38pp vs spot; the 2021–2026 backwardation era added +26pp on top of similar spot-index moves. See [[RollYield]].

## The 1973 Nixon price-freeze illustration (per Imsirovic)
The classical argument for why storage incentives *matter for macro policy*:
- During the 1973 Yom Kippur embargo, the Nixon administration **froze oil and product prices** across the board.
- Oil products are highly seasonal (gasoline/jet for summer, heating oil for winter). Freezing prices killed seasonality incentives — nobody has reason to store winter heating oil in February if the February price equals the December price.
- Result: **shortages that weren't about supply per se** — about the missing carry incentive that normally moves inventory across seasons. Refineries can't swing output 30% between gasoline and distillate overnight.
- Moral: the curve structure isn't decoration; it's the mechanism that funds inventory continuity through the year.

## The flat-price-vs-structure distinction
Both Imsirovic and [[RoryJohnston]] emphasize:
- **Flat price** encodes the *level* of scarcity (overall inventory position).
- **Curve structure** encodes the *pace* of inventory draw vs. build (rate of change).
- A fundamental modeling error (common in finance): using stored inventory as a *forecast* for flat-price, rather than recognizing that flat-price *causes* inventory changes.
- Imsirovic: *"The price of oil gets me to store oil or not. It's the other way around… Having said that, it's more complicated than that because the dynamic process, because anything in storage now is future supply."*
- Johnston's two-part framework: (a) the back-of-the-curve (36-month) flat price best predicts absolute inventory level (revealed-scarcity channel); (b) the front-minus-back spread predicts flow balance (theory-of-storage channel).

## The cost-of-carry link to monetary policy
- Storage is expensive: tank rental + insurance + capital + losses.
- **Interest rate = time value of money = a direct input to cost of storage.**
- Higher rates = higher carry cost = lower clearing price of oil in backwardation-steepening terms.
- Imsirovic: *"Volatility of the economic policy, volatility of monetary policy becomes a really big issue, because the traders that trade absolute price level on oil, they are clearly looking at interest rates."*
- This is how the [[OilPriceRecessionDebate]] intersects with microstructure: the market's pricing of cost-of-carry ratifies or overturns CB rate guidance, and Dec 2026 WTI became the forward-SOFR barometer precisely because of this link (see [[WTI]]).

## Connections
- [[AdiImsirovic]]
- [[IlyaBouchouev]]
- [[BrentComplex]]
- [[WTI]]
- [[CrackSpreads]]
- [[Supercontango]]
- [[OilPriceRecessionDebate]]
- [[RoryJohnston]]
- [[oilgroundup-adi-imsirovic]]
