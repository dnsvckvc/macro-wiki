---
title: "JPM Collar Trade (JPM Option Whale)"
type: concept
tags: [options, dealer-gamma, market-structure, jpm-whale, vanna, charm]
sources: [jumping-the-shark-again, vix-inversion-buying-bonds-japan-jpm-option-whale]
last_updated: 2026-04-12
---

# JPM Collar Trade (JPM Option Whale)

A large, tens-of-billions SPX structured fund operated by JPMorgan (with mirror strategies at other shops) that resets quarterly. Also referred to as the **"JPM Option Whale"** when viewed from the dealer side. Its options overlay is so large it routinely dominates index price action near expiry.

## Structure
- **Long** the S&P 500 in the underlying fund.
- **Buy** an OTM quarterly put spread (long a put ~10% OTM, short a put ~20% OTM).
- **Sell** an OTM quarterly call to finance the put spread.

Dealers on the other side are short the bought put, long the call, and delta-hedge dynamically.

## Two regimes — the key mechanic
Per [[KevinMuir]] in [[vix-inversion-buying-bonds-japan-jpm-option-whale]] (7 March 2026), the direction of the market into expiration flips the whole dealer-gamma sign:

### Normal regime — market rallies into the sold call
- Dealers are *long* the call that JPM sold → **long gamma**.
- They hedge by buying dips and selling rips.
- This *dampens* volatility and tends to **pin** the market to the strike.

### Current regime (March 2026) — market falls into the bought put
- Dealers are *short* the put that JPM bought → **short gamma**.
- They hedge by selling dips and buying rips — the opposite.
- This *amplifies* volatility rather than dampening it.
- Dealers are at **maximum short gamma** when spot sits *exactly* on the strike. Muir flags Thursday 5 March 2026's close right at **6475** (cash index) as that maximum-pain point.

## The three-greek squeeze (Friday 6 March 2026)
When spot breaks *through* the put strike, three greeks stack on the same side for the dealer:
1. **Gamma:** short — forces delta selling into weakness.
2. **Vanna:** rising vol requires additional selling to hedge cross-convexity.
3. **[[Charm]]:** **negative** when spot is below the put strike. Normally charm causes dealers to *buy back* futures as time passes (the put drifts OOM); below the strike, time itself adds *more* selling pressure.

Muir: *"There sure were lots of reasons market makers were scrambling on Friday."*

## Current incarnation
- **Strike:** 6475 on the SPX cash index (per Muir) — Paulo in [[jumping-the-shark-again]] references the same 6475 on the 31 March expiring future.
- **Expiration:** 31 March 2026 (quarterly roll).
- Muir: *"Once this trade is rolled on Tuesday [31 March], we should expect the market to settle down. This is currently a HUGE SOURCE OF INSTABILITY."*
- **The asymmetric tail both ways:** if [[DonaldTrump]] pumps the market with a "TACO" headline, dealers have to *chase the rally* just as hard as they chased the decline — violent squeezes in either direction.
- Paulo adds the compounding layer: add VIX call chasing ("wingy vanna protection") and 0DTE retail put buying and you get the full [[TurduckenOfMarketRisks]].

## Cross-author alignment
Muir (7 March) arrives at the mechanics-first explanation; Paulo (27 March) applies them in [[jumping-the-shark-again]]. Paulo quotes Muir directly: *"You have to have some frickin' balls to be a dealer managing that position right now."* Both authors view the 31 March expiration as the primary near-term instability window.

## Connections
- [[KevinMuir]]
- [[PauloMacro]]
- [[Charm]]
- [[TurduckenOfMarketRisks]]
- [[TomHanksHasCovidMoment]]
- [[DonaldTrump]]
- [[TrumpPumps]]
- [[AnatomyOfACrash]]
