---
title: "%clip"
---

# %clip

The `%clip` command (`%c` for short) creates a Twitch clip of the current moment. Once Twitch finishes processing it, the clip plays on the overlay.

```
%clip
%clip insane play
%clip insane play 20s
```

## Linking Your Twitch Account

Clips are created through your own Twitch account, so you have to link it first.
If you are not linked yet, `%clip` replies in chat with a link to connect your account; linking only grants permission to create clips.

## Title and Duration

Everything you type becomes the clip's title, up to 100 characters.

The last argument can instead be a duration: either an explicit one like `20s` or `1m`, or a bare number of seconds between 5 and 60.
Durations are clamped to **5-60 seconds**, and the default is **30 seconds**.

```
%clip that was crazy 15
```

## Rewards

Creating a clip rewards **5000 points** and **+50 karma**.

There is a 30-second cooldown, both global and per-user.

## On the Overlay

The clip appears on the overlay about 15 seconds after creation, tagged with who clipped it:

```
clipped by <username>
```

The clip link is posted in chat, and new clips are forwarded to the Discord clips channel by the bot.

Looking to replay someone else's clip instead? See [`%showclip`]({{< relref "showclip.md" >}}).
