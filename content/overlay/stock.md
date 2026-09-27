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

- **HEART** tracks vanor's heartrate. Higher heart rate means the stock goes up; lower heart rate means it goes down.
- **KRMA** (gold) tracks the channel's [karma]({{< relref "karma.md" >}}), mapped to a 0-100 price. High karma means an expensive stock; low karma means a cheap one.

## Buy Mechanics

Buying stocks can fail. The more you invest, the higher the risk.
You can use the `overpay` option to boost your odds.
Use [`%check %buy <symbol> <amount> [overpay]`]({{< relref "check.md" >}}) to preview the fail chance before committing points.

Both buying and selling have a 2-second cooldown.

## Check-In Bonuses

Using `%checkin` grants **1000 points** and **100 free shares** of HEART stock.
