---
title: "Stock Market"
---

# Stock Market

Order-book based stock market. Trade shares of stocks with other chatters.

- `%buy <stock> <amount> <price>` -- place a buy order
- `%sell <stock> <amount> <price>` -- place a sell order
- `%stocks` -- view your portfolio and open orders
- `%buyorders` / `%sellorders` -- see random orders on the book
- `%gamba` -- gamble spin (60s cooldown)

Orders match instantly when a counterparty order meets your price. Unmatched orders sit on the book until filled or the stream ends.

`%checkin` grants free shares in all stocks.

`%endstream` (broadcaster only) closes the market, pays out all holdings at last trade price, and refunds unfilled buy orders.
