---
title: "Basis Trade"
type: concept
tags: [rates, treasury, hedge-fund, arbitrage, market-structure]
sources: [making-macro-great-again-quick-updates, the-anatomy-of-a-crash, risks-of-another-financial-crisis-part-1, macrovoices-528-luke-gromen, treasury-qe-warsh-fed-eclipsed]
last_updated: 2026-04-27
---

# Basis Trade

A capital-intensive Treasury arbitrage run primarily by hedge funds: **buy slightly off-the-run cash Treasuries, short Treasury futures**. The trade captures the spread between cash and futures, earning the difference by delivering cheap cash bonds into the futures contract at expiry.

Asset managers are the main long in futures (it is more capital-efficient to own duration via futures than cash), while hedge funds supply the futures short. When hedge-fund short exposure contracts, either cash Treasuries or futures — or both — become harder to clear.

## Why it matters in [[the-anatomy-of-a-crash]]
Per [[PauloMacro]] (14 March 2026):
- Hedge-fund net short in futures has **declined by over 25%** in recent months — the basis trade is quietly unwinding.
- The confirmation is in [[SwapSpreads]], which have gone deeply negative (10Y / 30Y approaching Liberation Day levels). Deep negative swap spreads mean cash Treasuries are cheap vs swaps — a symptom of binding dealer balance-sheet constraints and arbitrage capacity being scarce.
- Paulo reads this as: *the basis trade is already under strain while nobody is talking about it*. When overnight rates still look well-behaved, it's easy to miss the fact that dealer balance sheets are actually tight.
- Rising Treasury-collateral volatility (e.g. the 2Y yield exploding 10bps over Fed Funds in a single day) is the mechanism that forces further [[Degrossing]] at multimanagers: when collateral whips, the "upside-down pyramid" of asset book on a collateral base cannot sustain high gross exposure.

## The Cayman Islands figure (per [[macrovoices-528-luke-gromen]])
The most load-bearing number on foreign UST demand: per an October 2025 Fed white paper, the **Cayman Islands accounts for 37% of net US Treasury note & bond issuance over the past 4 years.** That's almost entirely US hedge funds running the basis trade offshore. Implications:
- **Nominal "foreign demand" is at all-time highs** — but it's heavily levered hot money, not patient foreign central banks/pensions/insurers.
- Foreign central banks haven't bought net since 2014; they've switched to gold (long-term UST priced in gold is −90% since 2014).
- This hot-money base *sells* Treasuries when volatility rises. Treasuries have become **risk-off and risk-on assets simultaneously** — they no longer reliably diversify equities.
- [[LukeGromen]]: this is the structural vulnerability that makes the Treasury market especially fragile to any volatility pulse from the [[StraitOfHormuz]] crisis or the [[WallOfDebt]] refi wave.

## Structural context: Howell's [[DebtLiquidityRatio]] (per [[risks-of-another-financial-crisis-part-1]])
[[MichaelHowell]]'s framework explains *why* the basis trade is under stress at this particular moment: 77% of global lending is collateral-based (World Bank), mostly transacted via repo. The [[DebtLiquidityRatio]] is rising as the [[WallOfDebt]] arrives and the [[GlobalLiquidityCycle]] turns down. Collateral is getting structurally scarcer relative to the debt it supports. The basis trade — which relies on cheap collateral and tight spreads — is an early casualty of this mismatch.

## The Stealth-Accord moral-hazard view (per [[treasury-qe-warsh-fed-eclipsed]])

[[MichaelHowell]]'s 25 April 2026 piece adds the *coiled-spring* framing that brings Paulo's "quietly unwinding" observation, Gromen's Cayman Islands data, and the Stealth Accord into a single coherent picture:

> *"Hedge funds have become the marginal buyers of Treasuries. Foreign demand (currency hedged) has faded. Hedge funds use cash Treasuries as collateral to borrow in repo markets, funding leveraged derivative positions — basis trades, yield curve arbitrage, even crypto and stock futures. This compresses volatility like a coiled spring, but only for as long as repo markets stay stable."*

The moral hazard from the [[StealthAccord]]:
> *"Markets have come to expect Treasury buybacks whenever volatility rises. This can encourage excessive leverage in hedge fund basis trades. Why hedge and avoid volatility when the Treasury caps it for you?"*

The unwind chain (per Howell): SOFR spikes or haircuts rise → hedge funds face rapid deleveraging → forced selling of Treasuries into illiquid market. **March 2020 COVID is the precedent.**

The basis trade is now load-bearing in *both* directions:
- **Up:** as the marginal buyer of Treasuries, basis-trade leverage suppresses MOVE → expands the [[CollateralMultiplier]] → expands Global Liquidity. Bullish in calm regimes.
- **Down:** as the marginal seller in stress, the unwind feeds the same [[CollateralMultiplier]] mechanism in reverse — haircuts rise, re-hypothecation reverses, liquidity contracts mechanically.

This is the wiki's clearest explanation for *why* the [[StealthAccord]] is "ingenious but fragile": the same mechanism that creates effortless liquidity in calm regimes destroys it in crisis regimes.

## Connections
- [[PauloMacro]]
- [[SwapSpreads]]
- [[Degrossing]]
- [[RollingVARShock]]
- [[AnatomyOfACrash]]
- [[DebtLiquidityRatio]]
- [[WallOfDebt]]
- [[MichaelHowell]]
- [[LukeGromen]]
- [[StealthAccord]]
- [[TreasuryQE]]
- [[CollateralMultiplier]]
- [[MOVEIndex]]
