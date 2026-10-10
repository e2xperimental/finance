---
layout: post
title: How can I build my own index fund? 
date: 2026-10-09 10:00:00 -0000
category: "DIY index fund"
---
The index methodology determines whether it belongs in the index. Market-cap weighting then determines its weight.

So if you buy an S&P 500 ETF, you don't have to figure out whether Apple should be 6.2% or 6.4% tomorrow. The fund handles it.
Suppose you wanted to replicate the S&P 500:
1. Get the current S&P 500 constituent list.
2. Get each company's current index weight.
3. Decide how much money you want in your "personal S&P 500."
4. Calculate:
   
Dollar amount = Portfolio × Index weight

Then:

Shares to buy = Dollar amount ÷ Stock price

## Example with a $100,000 portfolio

Stock	Index weight	Target $	Price	Shares
Apple	6.5%	$6,500	$200	32.50
Microsoft	5.5%	$5,500	$400	13.75
Amazon	3.5%	$3,500	$200	17.50
...	...	...	...	...
Total	100%	$100,000		

If your brokerage supports fractional shares, you can get remarkably close to the index.

## The index providers publish the rules.

### S&P 500
S&P Dow Jones Indices publishes the methodology, constituent list, index weights, and announcements of changes. The S&P 500 is float-adjusted market-cap weighted and is reviewed/rebalanced quarterly.
[S&P Global](https://www.spglobal.com/spdji/en/methodology/article/sp-us-indices-methodology/)

S&P also explains the basic philosophy: stocks are added/deleted according to the index's eligibility and selection rules, generally through scheduled rebalancing, while corporate events can cause changes outside the normal schedule. [S&P Global](https://www.spglobal.com/spdji/en/research-insights/index-literacy/methodology-matters/)

### Russell 1000/2000
FTSE Russell publishes its construction methodology and reconstitution schedules. This is particularly interesting for your idea because Russell moved to semiannual U.S. index reconstitution beginning in 2026, in June and December, with quarterly IPO additions. [LSEG](https://www.lseg.com/en/ftse-russell/russell-reconstitution)

The Russell methodology even publishes the dates used to determine membership and when preliminary additions/deletions are released. [LSEG](https://www.lseg.com/content/dam/ftse-russell/en_us/documents/ground-rules/russell-us-indexes-construction-and-methodology.pdf)

### MSCI
MSCI also publishes index methodologies and maintains a searchable methodology database. Its indexes are generally rebalanced quarterly or semiannually depending on the index.
[MSCI](https://www.msci.com/indexes/index-resources/index-methodology)

## There's an even better way to do this
Rather than manually maintaining 500 stocks, you could create a "personal index" with perhaps 50–100 stocks.
For example, you could create:
DIY U.S. Total Market
- Large cap: 70%
- Mid cap: 20%
- Small cap: 10%
Or:
DIY S&P 500
- Select the 50–100 largest S&P 500 companies
- Weight them according to market capitalization
- Rebalance quarterly
The difference in diversification between owning 500 companies and, say, 100 companies can be surprisingly small if those 100 represent most of the market's capitalization.

## Another more interesting approach
Use the index's weights, but don't necessarily own every stock.
You could establish a minimum position size.
For example:
"I will own every S&P 500 company whose target weight is ≥0.25%, and ignore the tiny positions."

That dramatically reduces the number of trades while retaining most of the economic exposure.
