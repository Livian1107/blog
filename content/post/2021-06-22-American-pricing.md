+++
author = "Liwen"
title = "American option pricing"
date = "2021-06-22"
description = ""
tags = [
    "Fixed Income", "Bloomberg"
]
+++

Perpetual call/put
Finite call/put

Numerical solution
- Binomial tree: longstaff-schwartz
线性回归
Heat Equation

Digital American Option - Barrier Option

1. Perpetual American Put
no expiry date. -> infinite
payoff = max{0, K-St}
stock market: homogenity: 同质化

Value: stopping time 随机变量
if a random varible, e, satisfies {e<=t} for any t>=0
Then e is a stopping time.

frist hitting time - stock price drops to certain point, exercise the put

Stopped process

Theorem: a martingale, super martingale/sub-martingale stopped
at a stopping time is a martingale

### Put-call parity
Put-call parity: a principle that defines the relationship between the price of
European put and call options of the same class, that is, with the same 
underlying asset, strike price, and expiration date.

Put-call parity says the price of a call option implies a certain fair price for the corresponding
put option with the same strike price and expiration date. (and vice versa)

If the put-call parity is violated, then arbitrage opportunities are born

C + PV(x) = P + S

### How are options priced?
It is the sum of its intrinsic value, which is the difference between the current price
of the current price of the underlying asset and the option's strike pirce,
and time value, which directly related to the time left until that option's expiry.

Model:
Black-Scholes-Merton: BSM
input: strike price, current price of the underlying instrument, time to expiration, risk-free rate,
and volatility

This model will spit out the option's fair market value.

### Example
Protective put: a long stock position + a long put -> limit the downside of holding the stock
Fiduciary call: a long call + cash equal to the present value of the stike price -> ensures that 
the investor has enough cash to exercise the option on the expiration date.

### Why is put-call parity important?
- It allows you to calculate the approcimate value of a put or a call relative to its other components.
- If the principle violated, the prices of the put and call options fiverge so that an arbitrage opportunity exists.
- It offers opportunity for traders to theoretically earn a risk-free profit.
- It offers the flexibility to create synthetic positions.
