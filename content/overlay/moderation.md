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
`%restart`, `%block`, `%unblock`, `%refreshVoice`, `%rotate`, `%distract`

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
