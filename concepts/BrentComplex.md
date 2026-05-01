---
title: "The Brent Complex"
type: concept
tags: [oil, brent, futures, physical, term-structure, microstructure, imsirovic]
sources: [oilgroundup-adi-imsirovic, macrovoices-528-rory-johnston, macrovoices-529-ole-hansen]
last_updated: 2026-04-23
---

# The Brent Complex

The layered, historically-accumulated system of instruments that together price the global oil market via the Brent benchmark. Not designed top-down; grew over decades. Per [[AdiImsirovic]]: *"The most complicated commodity market in the world… like a human eye or body, with an appendix and molars sticking out… but it works."*

Anchored in [[oilgroundup-adi-imsirovic]] and used operationally across [[macrovoices-528-rory-johnston]].

## The five instruments

### Dated Brent (physical)
- Physical cargo with a **nominated loading date 10-30 days forward**.
- Assessed daily by PRAs (Price Reporting Agencies, e.g. Platts, Argus).
- The *physical benchmark* — what refineries actually pay for crude they'll run.
- This is the price that goes to $132/bbl when there's panic, while ICE futures stay near $100.

### Forward Brent (cash)
- Contract to deliver a physical Brent cargo at a future month (e.g. "December 2026 Brent").
- **How Brent trading originally started** — pre-futures, in the 1980s.
- Still the most important instrument for specialists; per Imsirovic: *"forward Brent is the most important instrument in Brent, and very, very few people know that."*
- CFDs settle to forward, not futures.
- US convention calls this "cash"; UK convention uses "cash" for forwards-not-yet-physical; the semantic gap confuses everyone.

### ICE Brent futures (paper)
- **Financially settled** (unlike WTI, which is physically deliverable).
- Normally trades **~2 months forward** (front-month is 2 months ahead of prompt cash).
- The "price on the screen" that virtually every non-specialist quotes as "oil."

### CFDs (Contracts for Differences)
- Swaps referencing **Dated Brent vs. Forward Brent** (not vs. futures).
- The mechanism by which dated cargoes price off a benchmark month.
- CFD curve traces continuity of the Dated-Brent time structure.

### EFP (Exchange of Futures for Physicals)
- The bridge between ICE futures and physical delivery.
- *"If you're long, 700,000 barrels of Brent on futures market in June, you can call your broker and say: I want to buy an EFP — normally under normal circumstances, you pay four or five cents a barrel and you will get a physical cargo from your futures. No problem."*
- **Normal EFP: 4-5 cents/bbl.**
- **Crisis EFP (June 2026 at peak):** >20 cents/bbl, coming back to 14-15 cents.
- An EFP ~4× normal is a simple quantitative signal of the paper-vs-physical premium divorced from curve shape.

## Why these are "not the same thing"
Imsirovic: *"It's apples and oranges — the same commodity in a very, very different time period."*
- Dated Brent is a physical barrel loading in **10-30 days**.
- ICE Brent futures reference a delivery month **~2 months forward**.
- Comparing them directly is category-confused. In backwardation, dated is *always* above futures; in contango, dated is *always* below.
- The spread between them is a function of curve shape + physical premium — not a market failure.

## The April 2026 price stack reconstructed
Working example from Imsirovic + [[macrovoices-528-rory-johnston]]:
- **Brent futures** (front-month, mid-April): ~$95-100/bbl.
- **+$30-32 Dated Brent** over futures.
- **+$15 Focados** (Nigerian distillate-rich crude) over Dated Brent.
- **+ ~$5 freight + insurance**.
- **= ~$150/bbl for a physically delivered distillate-rich barrel.**
- Extreme individual prints: **HSBC CEO's $286/bbl cargo to Sri Lanka.**

## June/December futures spread
- During the crisis: **~$20 backwardation** between June and December 2026 futures.
- Imsirovic: *"I can't remember ever seeing that."*
- Shows the backwardation isn't confined to the Dated-vs-futures divergence — it's present *inside* the futures strip itself.

## Why the curve doesn't "forecast" flat price
- Kevin Hassett (US) and [[IEA]]'s Fatih Birol quoted as implying the futures strip predicts future spot price (e.g., "futures curve says oil will be $70 next summer").
- Imsirovic's correction: the curve encodes **necessary seasonal storage incentives** — not a forecast. Gasoline/jet need summer storage built in winter; distillates need winter storage built in summer. The curve prices these incentives so the market carries inventory across time.
- Corollary: when resolution of the crisis arrives, *the whole curve shifts together*. The front doesn't collapse to the back; the back lifts with the front. Backwardation persists (Fujairah damage, shipping logistics, storage operational issues) even as flat price falls.

## Why this matters for the wiki
- **Explains the "forward curve hasn't repriced" puzzle** ([[AdamRozencwajg]]): paper is rationally pricing eventual OPEC-spare-capacity return, not denying the physical crisis. Imsirovic's complex-structure view is what makes Rozencwajg's observation consistent with functioning markets.
- **Anchors [[RoryJohnston]]'s $32 Dated-vs-futures observation** with mechanical explanation: it's the spread going to panic levels, not the paper market breaking.
- **Reframes Paulo's [[CrackSpreads]] rollover argument** from the physical-market side: the refinery-margin squeeze Paulo describes as a second-derivative signal *is* the same mechanism Imsirovic describes as the [[BrickAndMortarTrade]] — refineries paying whatever it takes for physical barrels.

## Connections
- [[AdiImsirovic]]
- [[WTI]]
- [[CrackSpreads]]
- [[TheoryOfStorage]]
- [[BrickAndMortarTrade]]
- [[AdamRozencwajg]]
- [[RoryJohnston]]
- [[IlyaBouchouev]]
- [[oilgroundup-adi-imsirovic]]
- [[macrovoices-528-rory-johnston]]
