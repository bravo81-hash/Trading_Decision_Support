# Trading Decision Support

Interactive single-file HTML app for index options position adjustment decisions.

## Scope

This app is designed around index options strategies on SPY, QQQ, SPX, RUT, and ES, including:

- ATM calendars / diagonals
- OTM dual calendars / diagonals
- OTM calendar + butterfly / broken-wing butterfly
- RUT put credit spread + OTM put calendar
- Triple calendars / diagonals
- OTM put broken-wing butterflies

## What it does

The app combines:

1. Hard guardrails
   - Final-hour execution rule
   - One-adjustment-per-day rule
   - Profit-target rule
   - Defensive drawdown mode
   - Hard -20% loss discomfort rule
   - Low-DTE complexity warning
   - RUT PCS danger rule

2. Weighted scoring
   - Delta imbalance
   - Market move severity
   - ATR multiple
   - Price location versus tent/breakeven
   - IV condition
   - Technical context
   - Event risk
   - Strategy-specific constraints

3. Transparent output
   - Primary recommendation
   - Confidence level
   - Ranked alternatives
   - Warnings
   - Avoid/deprioritise list
   - Score explanation

## How to use

Open `index.html` in a browser. No install or external dependencies are required.

## Important disclaimer

This is a decision-support tool only. It does not provide financial advice or trade instructions. Always model the adjusted risk graph, max loss, breakevens, liquidity, and order fills before placing any trade.
