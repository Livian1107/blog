+++
author = "Liwen"
title = "American option pricing"
date = "2021-06-22"
description = "Learning about ESG investing, ESG factors and why demand for sustainable and responsible investment is increasing."
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