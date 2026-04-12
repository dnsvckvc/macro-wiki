---
title: "VIX Inversion, Buying Bonds, Japan & the JPM Option Whale"
type: source
tags: [macro, vix, bonds, japan, dealer-gamma, jpm-whale, kevin-muir]
date: 2026-03-07
source_file: raw/raw/Clippings/VIX INVERSION, BUYING BONDS, JAPAN & THE JPM OPTION WHALE.md
---

## Summary
[[KevinMuir]]'s 7 March 2026 Q&A note ("Catching up with Kev, Part 2") covering four positions: (1) his US stock-index short and the [[VIX7v2Spread]] he watches for capitulation — it only just inverted on Thursday, nowhere near the −3/−4 level he wants before covering; (2) his **long fixed-income trade** across 2s, 5s, the long-end, and Canadian CORRA — front-end paper now carries positively for the first time in a long time, meaning he's "getting paid to take the 'Fed will be easier than expected' risk"; (3) his **long Japanese equities** position held for the long haul, with Japanese yen longs "too early" but unchanged; and (4) a detailed dealer-mechanics explanation of the [[JPMCollarTrade]] (which he calls the "JPM Option Whale"), flagging Thursday 5 March's close right at the 6475 strike as the moment dealers were *maximally* short gamma. Key line: *"This is currently a HUGE SOURCE OF INSTABILITY."*

## Key Claims

### VIX curve — not yet capitulated
- The widely-cited front-month VIX inversion is noise; the signal Muir watches is the **7th vs. 2nd VIX contract spread**.
- That spread held positive for an entire month and only flipped to inverted on Thursday 5 March 2026.
- He will start covering his index short only when the spread blows out to **−3 or −4**.

### Long fixed income — a qualitatively new trade
- 2Y yield has risen back above Fed Funds: the position now **carries positively** for the first time in a while.
- *"In the past, you needed to bet on more cuts than what were priced-in to 'win.' Today, all that needs to happen is there to be fewer hikes than what's priced-in."* Muir frames this as being *paid* to own the insurance asset rather than paying for it.
- Historical precedent: [[PaulTudorJones]] owned tons of 5Y T-notes into the 1987 crash; Morris Sachs / Greenwich Capital hit it big during LTCM with far-dated Eurodollar calls cheap off a steep curve.
- Current book:
  - Started with **5s** as a hedge against his short HY credit position.
  - Added **5Y call options** for bend / convexity.
  - Now owns "the whole curve" — including the long-end, which he'd previously avoided. Rationale from a trader friend: *"The bond market is the most contra market in the world. Whatever you think it should do, it does the opposite. No one owns the long-end. I bet it flies."*
  - Bought long-end calls "for a punt."
  - Majority of exposure at **2Y and 5Y**.
  - Added **Dec 2026 CORRA** (Canadian SOFR) futures — three BoC *hikes* are priced in; Muir: "Our economy will be crushed after the first hike."
- ETF suggestion: **Harley Bassman's TUA** — levers 2Y Treasuries to 10Y duration; now carries positively.
- Notes [[DavidRosenberg]] has given up on the long-end and focused on short-dated paper.

### Japan
- **Long Japanese stocks** held for the long haul; will only *add*, not touch the existing position. Energy worries already priced in.
- **Long Japanese yen** — admits he has been "too bullish way too early." Continues to trade from the long side but losing money. Will announce when he gives up, "so you folks can really load up."

### The JPM Option Whale — dealer mechanics
A detailed, mechanics-first explanation of what [[PauloMacro]] later calls the [[JPMCollarTrade]]:
- The fund sells an OTM quarterly *call* to buy an OTM quarterly *put spread*. Gargantuan size; routinely dominates index price action near expiry.
- **Normal regime:** market has rallied into the fund-sold call → dealers are *long* that call → long gamma → buy dips / sell rips → volatility dampens / market pins to the strike.
- **Current regime (March 2026):** market has fallen into the *put* strike at **6475** (cash index, expires 31 March) → dealers are *short* the put → **short gamma** → sell dips / buy rips → *amplifies* volatility.
- Thursday 5 March's close right at 6475 put dealers at their **maximum short gamma** position.
- Friday 6 March: dealers selling more deltas as they chased gamma; rising vol also forced **vanna selling**; unusually, **charm was negative** (see below).
- **Charm explainer:** charm is the change in delta from the passage of time. Above the put strike, charm causes dealers who are short the put + short futures to buy back futures as time passes (the put drifts OOM). *Below the strike*, charm is negative — the passage of time itself causes more delta selling, all else equal.
- Muir adds the Trump-tail scenario: if Trump "TACOs" and the market chases back through the strike to the upside, dealers have to chase it up just as hard as they chased it down — an asymmetric tail both ways.
- "Once this trade is rolled on Tuesday [31 March], we should expect the market to settle down. This is currently a HUGE SOURCE OF INSTABILITY."

## Key Quotes
> "The 7th vs. 2nd VIX Contract Spread… has steadfastly stayed positive, and it was only on Thursday that it finally flipped to inverted. If this spread blows out to minus 3 or minus 4, I will bring some of my short in."

> "In the past, I had to pay for that exposure. Now I am earning."

> "The bond market is the most contra market in the world. Whatever you think it should do, it does the opposite. No one owns the long-end. I bet it flies." — unnamed trader friend, quoted by Muir

> "This is currently a HUGE SOURCE OF INSTABILITY." — on the JPM Option Whale

> "I will tell you when I give up so you folks can really load up." — on his yen long

## Connections
- [[KevinMuir]] — author
- [[JPMCollarTrade]] — this piece is the canonical mechanics-first explanation; Paulo references it three weeks later
- [[VIX7v2Spread]] — Muir's preferred capitulation signal
- [[Charm]] — options greek explained inline for the dealer hedging case
- [[HarleyBassman]] — creator of the TUA ETF Muir recommends
- [[DavidRosenberg]] — cited on long-end bonds
- [[PaulTudorJones]] — historical precedent for the long-bonds-into-a-crash trade
- [[PauloMacro]] — implicit — same topic, three weeks later (Muir is the primary source for dealer mechanics Paulo builds on)
- [[CreditCycle]] — Muir's short HY credit position sits in this thesis
- [[AnatomyOfACrash]] — Muir's instability framing aligns with Paulo's master framework

## Contradictions
- None. Strongly complements [[the-anatomy-of-a-crash]] — this piece is written 7 March 2026, *one week before* Paulo's 14 March master essay, and already describes the 6475 dealer-gamma setup Paulo's [[jumping-the-shark-again]] (27 March) later applies to the same strike. The two authors are independently arriving at the same load-bearing observation about the JPM whale's March-31 expiration.
- **Nuance, not contradiction:** Muir's "once this trade is rolled on 31 March, the market should settle down" is a more bounded prediction than Paulo's broader "crash in days/weeks" call. The two views coexist if 31 March is itself the inflection point at which short-gamma pressure releases into an outright crash rather than resolving cleanly.
- **Reinforces** the wiki's long-Japan cross-link: Muir is *not* touching his long Japanese equity position and plans only to add — which neatly absorbs the "Japanese sellers of Western assets repatriating home" flow discussed in the overview.
