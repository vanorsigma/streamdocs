---
title: "Tax (Timeouts)"
---

# Tax (Timeouts)

Whenever a chatter is timed out; whether by a moderator, a command fumble, a [stock market]({{< relref "./stock.md" >}}) buy failure, a community vote kill, or the [gamba wheel]({{< relref "./gamba.md" >}}); they are subject to a **wealth tax** deducted from their [points]({{< relref "./points.md" >}}) balance. Taxed points flow into the [lottery]({{< relref "./lottery.md" >}}) pool.

## Tax Rate

The tax rate depends on how the timed-out user's point balance compares to the median wealth of currently checked-in chatters:

| Condition | Tax Rate |
|-----------|----------|
| Balance **exceeds** the check-in median | **1%** of points |
| Balance **at or below** the check-in median | **0.1%** of points |

The tax is deducted from liquid vanorDollars only (stock holdings are untouched). If the user has no points, nothing is deducted. The deduction is capped so the balance never goes below zero.

Tax events are broadcast in chat, showing the amount deducted and the rate applied.

## Mods

Since moderators cannot be timed out by Twitch, the system handles them differently:

- When a mod would be the target of a timeout (e.g. from the gamba wheel), no actual ban is issued.
- Instead, the mod receives a **flat 20% tax** on their points, with no gun animation.

## Broadcasters

Broadcasters are immune from the tax system. They are never timed out and never taxed.
