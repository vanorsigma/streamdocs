---
title: Gamba Wheel
---

# Gamba Wheel

Triggered with `%gamba <amount>`.

TODO: insert screenshot here, ideally showing the wheel mid-spin.

The gamba wheel is a weighted random spin. You can win or lose points.
The amount you wager multiplies the outcome values.

You spin with `%gamba <amount>`, which deducts the wager from your [points]({{< relref "points.md" >}}).

The wheel has a 60-second global cooldown and a 30-second per-user cooldown.

## Possible Outcomes

The wheel can land on a mix of good and bad outcomes:

- **Points**: receive points. The amount is a positive or negative multiplier on your wager.
- **Stock grants**: receive free [stock market]({{< relref "stock.md" >}}) shares.
- **Channel point redeem triggers**: activates a random channel point redeem.
- **Timeout**: times you out for a duration. The timeout duration is **not** scaled by your wager. Being timed out also triggers a [tax]({{< relref "tax.md" >}}) on your points.
- **Everyone points/stocks**: gives points or stock to all checked-in chatters.
- **Increased chances**: temporarily boosts command success chance for all chatters.
- **Cooldown resets**: resets your cooldowns or everyone's cooldowns.

Subscriptions, bit donations and [watch streaks](#watch-streak-gamba) spin different wheels with better odds.

Gamba spins also queue up. If multiple people spin at once, they are processed one at a time.

## Watch Streak Gamba

When a chatter shares a [Twitch watch streak](https://help.twitch.tv/s/article/viewer-milestones), they get a free gamba spin if their streak hits a multiple of the configured interval (default: every 5). The wager equals `streak * 100` points and is free (not deducted from balance).

Possible watch streak outcomes:

- Receive points (100, 500, or 1000)
- Everyone receives points (250)
- Everyone receives HEART stock (100 shares)
- Everyone gets increased command success chance (+10%)
- Reset all cooldowns
- Receive HEART stock (100 shares)

Watch streaks and the streak interval can be configured in the Captain dashboard.
