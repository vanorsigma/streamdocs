---
title: Lottery
---

# Lottery

Triggered with `%lottery [amount]`.

Run `%lottery` with no arguments to see the current pool size and participant count.

The lottery is a communal point pool that grows from entry fees and timeout [taxes]({{< relref "tax.md" >}}). The broadcaster draws a winner using a weighted gamba wheel spin.

## Entering

Bet points with `%lottery <amount>`. Your points are deducted from your balance and added to the pool as **shares**. More shares means better odds of winning.

```
%lottery 500
```

You may enter multiple times. A 60-second per-user cooldown applies between lottery entries.

## Payout

Only the broadcaster can trigger the payout:

```
%lottery payout
```

This consumes the pool (entries + accumulated taxes), clears all lottery state, and spins the [gamba wheel]({{< relref "gamba.md" >}}) weighted by each participant's shares. The wheel announces the winner and awards them the full pool.

If no one has entered, the payout command does nothing.

## Pool

The pool is the sum of:

- All lottery entry points
- Timeout [tax]({{< relref "tax.md" >}}) revenue collected since the last payout

The pool grows passively as chatters get taxed. Entering the lottery does not grant your pool contribution to anyone -- only the winner takes all.

## Ties

If multiple participants have identical shares, the gamba wheel weight distributes odds evenly across them.
