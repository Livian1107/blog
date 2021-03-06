+++
author = "Liwen"
title = "Negotiation starter(answer）- How to split the wine bill?"
date = "2021-03-06"
description = "Detailed solution to wine bill negotiation."
tags = [
    "Negotiation - Yale", "Game Theory", "Coursera",
]
+++

##### Recap of the wine bill negotiation.
---

Andrea and Beth are dining at a fine restaurant. There is a bottle of 2009 Grgich Hills Chardonnay on the menu and the price is $100. To keep things simple, albeit unrealistic, assume the restaurant only sells whole bottles and this is the only wine they carry.

* Andrea would be willing to pay $110 to drink the whole bottle.
* Andrea would be willing to pay $90 to drink half the bottle.
* Beth would be willing to pay $80 to drink the whole bottle.
* Beth would be willing to pay $50 to drink half the bottle.

They would like to share a bottle if it makes sense to do so (and if they can agree on how to divide the costs). To see if it makes sense, what is the pie, in dollars?

---
#### Solution
The key to the negotiation is to find out what's the PIE?

##### Valuations
|        | Whole Bottle | First Half Bottle | Second Half Bottle |
|--------|:------------:|:-----------------:|:------------------:|
| Andrea | $110         | $90               | $20                |
| Beth   | $80          | $50               | $30                |

Beth values a half bottle at $50 while Andrea values seconde half at $20. Beth's valuation is $30 more than what Andrea values the second half.
__Hence PIE is $30.__ Andrea would sell at $20 and Beth would pay $50. Splitting the gains means Beth pays $35 to Andrea. __Hence Andrea's net cost is $100 - $35 = $65.__

##### BATNAs
|        | Whole Bottle Valuation | Original Price | Gain |
|--------|:----------------------:|:--------------:|:----:|
| Andrea | $110                   | $100           | $10  |
| Beth   | $80                    | $100           | $0   |

If no deal, Andrea buys the whole bottle and is $10 ahead. Beth does not buy bottle and so is $0 ahead. Combined value if no deal is $10 + $0 = $10.

|        | First Half Valuation | Original Price | 
|--------|:--------------------:|:--------------:|
| Andrea | $90                  | $100           | 
| Beth   | $50                  | $100           | 

If deal, combined value of bottle is $140. Gain if cooperate is $40.

Therefore, PIE is $40 - $10 = $30. Split pie and each should be up to $15.

##### Reservation Price
Even Andrea is willing to pay $90 for half but she is not prepared to pay half at $90.
Andrea makes $10 buying full bottle. Hence reservation price(the most she will pay) for half bottle is now $90 - $10 = $80. Unless she pay less than $80, she could gain more from paying half bottle.
* Beth is up $15 -> Beth pays $50 - $15 = $35
* Andrea is up $15 -> Andrea pays $80 - $15 = $65
Gain is form reservation price.

---
#### Practice
New situation:
* Andrea would be willing to pay $160 to drink the whole bottle.
* Andrea would be willing to pay $90 to drink half the bottle.
* Beth would be willing to pay $80 to drink the whole bottle.
* Beth would be willing to pay $50 to drink half the bottle.

What's the PIE here?

|        | Whole Bottle | First Half Bottle | Second Half Bottle |
|--------|:------------:|:-----------------:|:------------------:|
| Andrea | $160         | $90               | $70                |
| Beth   | $80          | $50               | $30                |

If no deal, gain = $160 + $0 - $100 = $60.

If deal, combined value of bottle is $90 + $50 = $140, gain = $140 - $100 = $40.

Hence PIE = $40 - $60 = -$20.

However, this is not correct as it is better to have no deal to make PIE = $0. Second half bottle valuation to Andrea is $70 while half bottle is only $50 to Beth. 
Devaluation of the half bottle make it better to have no deal. 


###### Note: All the materials are shared for learning purpose, originally from Yale University lecturer @ Barry Nalebuff.

