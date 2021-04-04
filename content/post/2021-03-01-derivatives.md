+++
author = "Liwen"
title = "CFA I - Derivatives"
date = "2021-03-01"
description = "Notes from Coursera"
tags = [
    "CFA I",
]
+++

### Overview of derivative instrument and market

#### Define derivatives
A derivative is a financial instrument, special, differnt from tranditional financial instrument like stocks.

* A derivative derives its performance from _the performance of an underlying asset_. 本质上是一个赌约，关于参照物/标的资产的表现。
* Tranditional financial instrument, like stocks, benefits from future free cash flow, dividend.

Financial asset: equity股指期权, fixed-income security固定收益/国债, currency外汇 -> financial derivatives 
Physical asset: commodity 大宗商品
Other: interest rate利率, credit信用质量(CDS), weather, other derivatives, etc.

*CME, Chicago Mercantile Exchange -> trade weather derivatives

Derivative usually __transform__ (not simply pass through) the performance of the underlying asset before paying it out in the 
derivatives transaction.

Mutual fund is a channel to invest in underlying asset -> it is different from derivatives.
*Funds are not derivatives, they are simply pass through, instead of transforming

Derivatives are created in the form of legal contracts:
* The long: buyer, holder   -> in hope of price increasment  多
* The short: seller, writer -> in hope of price decreasement 空
** Option seller = Option writer

Example:
More than price, Person A buys bond: A is long bond price; A is short interest rate;
** Bond and interest rate are negatively correlated to each other. 债券和利率呈负相关 **

#### Contrast forward commitments with contingent claims 权利义务是否对等
##### Forward commitment 远期协议 （权利和义务）必须执行
Contracts entered into at one point in time that __require__ both parties to engage in a transaction at a later point
in time (the expiration) on terms agreed upon at the start. (Forward, futures, and swap)

Forward commitments provide linear payoffs.

##### Contingent claim 或有索求权（只有权利没有义务）
交易是否执行是不一定的
Derivatives in which the outcome or payoff is dependent on the outcome or payoff of an underlying asset. (Option)

#### Distinguish between exchannge-traded and over-the-counter derivatives (场内/场外)
##### Exchange-traded markets
Characteristics:
* Standardized
* No default risk - guaranteed by clearinghouse 没有违约风险
* Regulated
* Transparent
* High liquidity

Instruments:
* Futures
* Some options

In a forward contract, either party could default. Whereas in a contingent claim, default is possible only from the short to the long.

##### Over-the-counter (OTC) markets
Characteristics:
* Customized
* Default risk/counterparty risk 面临违约风险
* Unregulated
* Less transparent
* Low liquidity

Instruments:
* Forward
* Swap
* Some options

### Forward, futures and swap
* Define forward contracts, futures contracts, swaps, and compare their basic characteristics

#### Forward - zero sum game
Agreement between counterparties with different views.

An over-the-counter derivative contract in which two parties agree that one party, the buyer, will puchase
an underlying asset from the other party, the seller, at a later date at a fixed price they agree on when the contract is signed.

In addition to the (forward) price, the two parties also agree on several other matters, such as the identity and the quantity of the underlying.

There is no fee to paid on the forward contract. Counterparties dont owe each otehr anything as the price is on agreement.

|   | Forward Market | Spot Market |
|---|:--------------:|:-----------:|
| A | short          | long        |
| B | long           | short       |

Hedge, 进入相反的头寸，lose money in spot market while make money in forward market. Lower the risk of price changes


Ex1:

Ex2:

Forward contracts can be settled in two ways:
* Physical delivery: Delivery of the underlying asset
* Cash settlement: Exchange of cash: non-deliverable forwards (NDFs), cash-settled forwards, or contracts for differences.

Forward contracts can be structured to create a perfect hedge (market risk only, credit risk still exists), providing an assurance that the underlying asset can be bought
or sold at a price known when the contract is initiated.

Dealer: provide liquidity, a dealer creates a derivative contract and will quote a price to take a long or short position.
End user: an end user is typically a corporation or institution seeking to transfer an existing risk.

Default risk: 毁约风险
中小企业难以进入Forward市场

#### Futures - no default risk
Futures contracts are specialized forward that have been standardized and trade on a futures exchange

Futures contracts have specific underlying assets, times to expiration, delivery and settlement conditions, and quantities.

The exchange offers a facility in the form of a physical location and/or an electronic system as well as liquidity provided by authorized market makers.

* Futures price: the agree-upon price
* Price limit: a provision limiting price changes, establish a band relative to the previous day's settlement price, within which all trades must occur.
** limit up/down
** locked limit

Mark-to-market: daily settlement of gains and losses to margin account according to the settlement price

Settlement price: an average of the final futures trades of the day

Initial margin

Maintenance margin

Margin call


Long: SP>FP gain; SP<FP loss
Short: SP>FP loss; SP<FP gain

327国债

* Margin account： covers possible future losses, no formal load created as in equity market
* Equity margin account 保证金账户: an investor deposits part of the cost of the stock and borrows the remainder at the rate of interest

开仓: 无->有;多头开仓，多头平仓（卖掉现有仓位）
平仓: 有->无;空头开仓，空头平仓
锁仓：多头账户开空头合约，交了两份保证金
Offset/close-out: 
Open interest:

Forward vs. Futures:
* Forward contracts realize the full gain or loss at expiration
* Futures contacts realize the gain or loss in parts on a day-to-day basis
Time value of money differs


#### Swap
OTC derivative contract in which two parties agree to exchange __a series of cash flow__ whereby one party pays a variable series that will be determined by an underlying asset or rate and
the other party pays either 1) a variable series determined by a different underlying asset or rate or 2) a fixed series

**A swap is a series of (off-market) forwards

Characteristics:
* Custom instruments
* Not traded in any organized secondary market
* Largely unregulated
* Default risk is a concern
* Most participants are large institutions
* Private agreements (less transparent)
* Difficult to alter or terminate

More standardized -> more liquidity
more customized -> less liquidity in secondary market

* Interest rate swap: fixed for floating (plain vanilla); floating for floating
* Equity swap
* Currency swap


Plain vanilla interest rate swap


Forward: payoff, delivery;
Futures: standardized forward, daily settlement, margin;
Swap: a series of forward, interest rate swap;


#### Options 
A derivative contract in which one party, the buyer, pays a sum of money to the other party, the seller or writer, and receives
the right to wither buy or sell an underlying asset at a fixed price wither on a specific expiration date or at any time prior to the expiration date.

An option is a right, but not an obligation
Default in options is possible only from the short/seller to the long/buyer

Option premium: payment to seller from buyer
Call option: right to but, 看涨/认购, C0
Put option: right to sell, 看跌/认沽, P0
Exercise price/strike price(X): 
European option: exercisable at or prior to expiration, more expensive
American option: exercisable only at expiration
百慕大期权：介于欧式美式之间，允许中间提前行权但不是任意时刻

Moneyness (X: exercise price; St: spot price at time t):
* in the money实值/价内-》行权
* at the money在值/平值-》不行权
* out of the money虚值/价外-》不行权

Premium 期权费是沉没成本 不应予以考虑


#### Credit derivatives
credit default swap-put ooption


### Purpose of Derivatives
* Risk allocation, transfer and management
* Information discovery
** Price discovery
** Implied volatility
* Operational advantages
** Lower transation cost
** Greater liquidity
** Easy to go short
* Better market efficiency

Controversies
* Speculation and gambling
* Destabilization and systemic risk
* Complexity
* High leverage - too risky

### Pricing the derivatives
Arbitrage 套利
Replication
Risk neutrality

Present value of discounted cash flow (DCF)

The value of the financial asset = Expected future price + interim payments (e.g. dividends or coupon interest, discounted at a rate appropriate for the risk assumed)
E(St) + interim cash inflow (dividends) - interim cash outflow 

* Arbitrage空手套白狼：
1. no risk
2. no investment无初始投资

Law of one price: assrts that produce identical future cash flows

* Replication
An asset and hedging position of derivatives on the asset 

Asset + Derivative = Risk-free asset
Asset - Risk-free asset = -Derivative
Long asset, short bond, long forward 
