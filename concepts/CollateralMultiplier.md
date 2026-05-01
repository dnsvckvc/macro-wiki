---
title: "Collateral Multiplier"
type: concept
tags: [liquidity, collateral, repo, dealer-banks, move, basis-trade, howell, framework]
sources: [treasury-qe-warsh-fed-eclipsed, crypto-gold-pboc-vs-fed, risks-of-another-financial-crisis-part-2]
last_updated: 2026-04-27
---

# Collateral Multiplier

[[MichaelHowell]]'s quantitative framework ([[treasury-qe-warsh-fed-eclipsed]]) for *how Global Liquidity is created from the collateral pool* — the technical core of the modern repo-/collateral-based liquidity system.

## The identity

```
Global Liquidity ≈ Collateral Pool × Collateral Multiplier
$190 trillion    ≈   $150 trillion  ×    ~1.1×
```

The collateral pool is the value of Treasuries and other high-quality assets pledged into the repo / prime-broker / re-hypothecation system. The multiplier is the "M1 → M2" analog for collateral — how many derived liquidity dollars are produced per posted-collateral dollar.

## The two margins

The multiplier is determined by:

- **Intensive margin** = the *haircut* dealer-banks apply to posted collateral. A 2% haircut on a $100 Treasury = $98 of liquidity. A 10% haircut = $90 of liquidity.
- **Extensive margin** = *re-hypothecation* — how many times the same collateral is re-lent within the system. Higher re-hypothecation = larger multiplier.

Both margins are **strongly anti-correlated with bond volatility**:
- High vol → bigger haircuts → smaller intensive margin.
- High vol → less willingness to re-hypothecate → smaller extensive margin.

## The empirical rule

> **MOVE / collateral-multiplier correlation: −0.67**
>
> **Each 10-point fall in MOVE → ~$3 trillion (1.5%) of additional Global Liquidity.**

This is the wiki's clearest single-number explanation for why [[MichaelHowell]] cares so much about the [[MOVEIndex]] sitting around 80 — and why suppressed bond vol is *automatic stealth liquidity creation*.

> *"A lower MOVE index virtually assures automatic liquidity creation, regardless of where the Fed sets rates."*

## The pro-cyclical feedback loop

The multiplier mechanism creates **two-way amplification**:

| MOVE direction | Collateral multiplier | Global Liquidity | Risk-asset implication |
|---|---|---|---|
| Falls 10pts | Expands | +$3T | Bullish |
| Rises 10pts | Contracts | −$3T | Bearish |
| Spikes (e.g. geopolitical shock) | **Collapses mechanically** | Sharp contraction | March 2020-style spiral |

The mechanical-collapse case is the [[StealthAccord]]'s central fragility: the same mechanism that creates effortless liquidity in calm regimes destroys it in crisis regimes. The expected response (Treasury buybacks) is itself moral-hazard fuel that has built up larger leveraged positions ([[BasisTrade]]) which would deleverage the spiral.

## How Treasury QE leverages the collateral multiplier

Per Howell's framework ([[TreasuryQE]]):
- Treasury buyback volume responds to MOVE: ~$30bn per 10pt rise.
- That buyback compresses MOVE.
- MOVE compression expands the collateral multiplier.
- Multiplier expansion = ~$3T additional Global Liquidity per 10pt MOVE move.

The implied lever:
```
$30bn of buybacks → 10pt MOVE compression → $3T Global Liquidity creation
≈ 100× leverage
```

This is *why* Treasury QE has eclipsed Fed QE as the marginal liquidity driver in the [[StealthAccord]] regime — and why setting Fed funds is now *"a pantomime, a sideshow"* (Howell).

## Cross-reference to [[risks-of-another-financial-crisis-part-2]]

This 25 April piece formalizes what the 4 April [[risks-of-another-financial-crisis-part-2]] essay had described qualitatively: *"liquidity creation needs quality debt as collateral → transacted via repo (~$10–12T in US alone) → when disrupted: SOFR-IORB spread spikes, MOVE index jumps. Higher bond vol → bigger haircuts on collateral → reduced collateral multiplier → shrinking liquidity. This is the pro-cyclical feedback loop."*

The 25 April piece adds the **−0.67 correlation** and the **$3T per 10pt** sensitivity — making the 4 April qualitative loop quantitatively tradeable.

## Implication for the [[BasisTrade]] / [[LukeGromen]]

[[LukeGromen]]'s observation in [[macrovoices-528-luke-gromen]] — that 37% of net UST issuance over the past four years has gone to Cayman Islands hedge funds running the basis trade — is the **collateral-pool-input side** of Howell's framework. Patient sovereign holders have left; levered hot money has filled the gap. The collateral pool itself is now structurally pro-cyclical: it grows when MOVE is low (basis trades expand), contracts when MOVE is high (basis trades unwind). Combined with the multiplier-side pro-cyclicality, the system has *two-way amplification* compounded.

## Connections
- [[MichaelHowell]]
- [[StealthAccord]]
- [[TreasuryQE]]
- [[MOVEIndex]] — the input variable.
- [[BasisTrade]] — both the moral-hazard target and the collateral-pool input source.
- [[GlobalLiquidityCycle]] — the macro overlay; this is the micro-mechanism.
- [[LiquidityMechanics]] — Paulo's TGA/RRP/bank-reserves framework now sits at the *previous* layer; this framework sits at the binding-constraint layer.
- [[DebtLiquidityRatio]] — the systemic-risk aggregator.
- [[ReserveManagementPurchases]] — the Fed-side counterpart whose effect is mediated through *this* mechanism.
- [[LukeGromen]] — the basis-trade / Cayman Islands collateral-pool-input data.
