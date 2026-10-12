---
layout: post
title: A better way to build your own index fund 
date: 2026-10-11 10:00:00 -0000
category: "DIY index fund"
---

# There's an even better way to do what you're describing

Rather than manually maintaining 500 stocks, you could create a **"personal index" with perhaps 50–100 stocks**.

For example, you could create:

**DIY U.S. Total Market**

- Large cap: 70%
- Mid cap: 20%
- Small cap: 10%

Or:

**DIY S&P 500**

- Select the 50–100 largest S&P 500 companies
- Weight them according to market capitalization
- Rebalance quarterly

The difference in diversification between owning 500 companies and, say, 100 companies can be surprisingly small if those 100 represent most of the market's capitalization.

But there's another approach I think is particularly interesting for you.

### Use the index's *weights*, but don't necessarily own every stock.

You could establish a minimum position size.

For example:

> "I will own every S&P 500 company whose target weight is ≥0.25%, and ignore the tiny positions."

That dramatically reduces the number of trades while retaining most of the economic exposure.

---

## There are also tools that can automate the concept

For example, [M1 Finance](https://m1.com/?utm_source=chatgpt.com) has **Custom Pies**, where you assign target percentages to individual stocks and funds. M1 can then direct new deposits toward underweight positions and supports fractional shares. :chatgpt-content-reference{index="6"}

That's conceptually very close to what you're describing, although you'd still have to determine and maintain the index weights yourself.

---

# Here's where I think this gets really interesting for you

Given that you've been looking at **VTSAX, VTEB, VTES, cost basis, and DIY portfolio construction**, I'd be willing to build you a **Google Sheets "DIY Index Fund" calculator**.

It could have:

**Sheet 1 — Index Holdings**

| Ticker | Company | Index Weight | Current Price | Target $ | Shares Needed | Current Shares | Buy/Sell |
|---|---|---:|---:|---:|---:|---:|---:|

**Sheet 2 — Rebalancing**

You enter your portfolio value and current holdings, and it tells you:

> **BUY 3.42 AAPL**  
> **BUY 1.17 MSFT**  
> **SELL 0.63 NVDA**  
> **BUY 8.21 AMZN**

You could also establish a **5% tolerance band**, so it doesn't tell you to trade every time the market moves:

> Don't rebalance unless a position is more than ±5% away from its target.

And we could make it specifically follow **S&P 500, Russell 1000, Russell 2000, or another public index methodology**.

### One major advantage for you

If this is done in your **taxable brokerage account**, direct ownership gives you something an index mutual fund/ETF doesn't: **you can control which individual positions you sell.**

That potentially gives you more flexibility for **tax-loss harvesting and tax-efficient withdrawals**, which fits particularly well with the tax-diversification ideas you've been exploring.

The tradeoff is that you're taking on the administrative work that the ETF's ~0.03% expense ratio is paying someone else to do.

If you want, I can :chatgpt-content-reference{index="8"}, including :chatgpt-content-reference{index="9"}, and :chatgpt-content-reference{index="10"}.
