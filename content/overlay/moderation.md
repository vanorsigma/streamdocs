---
title: Moderation
---

# Moderation

Moderators can manage commands and chatters through community bids and direct actions.

## Blocking Commands

Commands can be blocked or unblocked with a community bid.

Start a bid with `%block <%command>` or `%unblock <%command>`. This opens a yes/no vote.
Chatters contribute points to the bid.
When the bid closes and succeeds, the command is blocked or unblocked.

The minimum bid is **1000 points**.

Some commands are **unblockable** and cannot be affected:
`%restart`, `%block`, `%unblock`, `%refreshVoice`, `%rotate`, `%distract`, `%important`, `%unimportant`, `%raid`, `%moment`

## Vote Kills

Moderators can start a community vote to timeout a user:

```
%kill <username>
```

This opens a yes/no bid targeting **2000 points**.
If the vote passes, the user is timed out.

## Reset Cooldowns

```
%resetcooldown [username|all]
```

Resets command cooldowns.
- No argument: resets your own cooldowns (free)
- A username: resets that user's cooldowns (costs 20000 points)
- `all`: resets all overlay cooldowns (mod only)

## URL Approval

When a user posts an image or audio URL through `%showimage` or `%playaudio`, a moderator may need to approve it before it appears.
A moderator (or the VIP who owns the command) must type the approval text in chat.

The moderator list is set in the overlay configuration.

## VIPs and Karma

Moderators and VIPs usually don't pay point costs for their own commands. Their commands still affect [karma]({{< relref "karma.md" >}}) though.

## Important Mode {#important-mode}

Important mode (`%important`) is an emergency toggle that pauses the entire stream experience. When activated:

- The **overlay hides** with a light-bulb + glow animation, fading to invisible.
- **All commands** (both overlay and Captain commands) are blocked, except `%unimportant`, `%moment` and `%raid`.
- **TTS** is disabled.
- **Kiki and Maki** (the AI agents) are paused; they stop receiving new inputs and stop speaking.

A countdown timer (opacity 0.25) appears in the top-right of the screen for the remaining duration.

### Permissions

- **VIPs**: can activate `%important` **once per stream** (per overlay restart).
- **Mods & broadcaster**: can activate it **unlimited times** and **turn it off** with `%unimportant`.
- **`%unimportant`** immediately restores the overlay, TTS, commands, and AI agents.

### Recovery

If the overlay tab crashes while important mode is active:

- The broadcaster can type `%unimportant` in Twitch chat. This is also a **Captain command** (server-side), so it works even without the overlay.
- The "End Important Mode" button on the Captain dashboard provides a manual fallback.

### Syntax

```
%important 5m       # 5 minutes
%important 30s      # 30 seconds
%important 1h       # 1 hour
%important 1m30s    # 1 minute 30 seconds
%unimportant        # End important mode immediately
```
