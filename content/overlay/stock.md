---
title: "Stock Market"
---

# Stock Market

The stream has a stock market. Invest [points]({{<relref "points.md" >}}) to grow them.

- `%invest <amount>` -- buy in at current price
- `%uninvest <amount>` -- sell at current price

The stock price tracks vanor's heart rate (HR). When HR rises (excitement, blushing) the price goes up. When HR drops (despair, calm) the price goes down.

The [model page]({{<relref "../model.md" >}}) shows HR thresholds for blush/despair.

Stocks reset on overlay restart unless vanor closes the market cleanly with `%closemarket`.
