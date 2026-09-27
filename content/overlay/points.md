---
title: Points
---

# Points

There is a custom point currency used to run [stream commands]({{< relref "../commands.md" >}}).

## Earning Points

Points can be earned in several ways:

- vanor gives them to you directly
- Through [CAPTCHA]({{< relref "./captcha.md" >}}). 500 points per claim.
- Through the [stock market]({{< relref "./stock.md" >}}). Buy low, sell high.
- Through `%checkin`. 1000 points once per overlay restart.
- Through the [gamba wheel]({{< relref "./gamba.md" >}}), if you get lucky.
- Through the [lottery]({{< relref "./lottery.md" >}}), if you win the pool.
- Through `%clip`. 5000 points for each clip you create.
- Through `%moment`. 10000 points for each moment.
- Through channel point redeems (if configured)

## Transferring Points

You can send points to another chatter:

```
%transfer <username> <amount>
```

This deducts the amount from your balance and adds it to theirs.

## Checking Balance

```
%points [username]
```

Shows your current balance, or another user's if you provide a username.

The richest chatters are tracked and displayed on the overlay's right panel.
