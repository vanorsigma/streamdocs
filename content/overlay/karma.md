---
title: Karma
---

# Karma

The Karma system is a global chat-wide currency affected by both command usage and [Kiki]({{< relref "kikimaki.md" >}}), the AI cat.

{{< figure src="/karma_1.png" title="Karma Scale, showing total karma to be 376.52, with +1.00 from Kiki" >}}

The karma value is displayed as a scale of justice on the overlay.

## Range and Thresholds

Karma ranges from **-5000 to +5000** and decays over time at a rate of **1% per cycle**.

When karma reaches **+250 or higher**, a "ding" notification plays on stream.

## How Karma Changes

Kiki uses her own judgement to issue karma for messages she chooses to react to, on a scale from **-500 to +50**.

Commands also affect karma. Refer to [Stream Commands]({{< relref "../commands.md" >}}) for per-command values.
Positive karma commands include `%blacksilence`. Most other commands consume karma.

The model blend shape toggles (`%hearts`, `%stars`, `%undress`) each consume a set amount of karma:
- Hearts: 5 karma
- Stars: 5 karma
- Undress: 50 karma

Bits and subscriptions also contribute positive karma.
