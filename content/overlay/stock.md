---
title: "Stock Market"
---

# Stock Market

The stream has a stock market where you can invest [points]({{< relref "points.md" >}}) tied to vanor's heartrate.
Stocks are the easiest way to earn points, but they are **lost on restart**. Your holdings disappear unless vanor closes the market before restarting.

TODO insert an image here

The market cycles every 15 seconds. Prices update from vanor's heart rate.

## Commands

|command|description|
|---|---|
|`%buy <symbol> <amount> [overpay]`|Invest `<amount>` points in a stock. Use `all` for your full balance. Add `overpay` to increase your chance of a successful buy.|
|`%sell <symbol> <amount>`|Sell your stock holdings. Use `all` to sell everything.|
|`%stocks`|View your current stock portfolio, including profit/loss.|

## Available Stocks

Currently, the only available stock is **HEART**, which tracks vanor's heartrate.

Higher heart rate means your stock goes up. Lower heart rate means it goes down.

## Buy Mechanics

Buying stocks can fail. The more you invest, the higher the risk.
You can use the `overpay` option to boost your odds.

Both buying and selling have a 2-second cooldown.

## Check-In Bonuses

Using `%checkin` grants **1000 points** and **100 free shares** of HEART stock.
