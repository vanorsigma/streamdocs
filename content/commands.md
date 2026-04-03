---
weight: 10
title: "Stream Commands"
---

# Stream Commands

There are several kind of commands.

## StreamElement Commands

This have no effect on the stream, and are usually either mod commands or commands displaying information.

- `!discord` - Shows discord
- `!sfx` - Shows a list of possibel sound effects
- `!piss` - The piss copypasta
- `!docs` - The docs copypasta

## Standard Overlay Commands

These are commands everyone can run with no special effects.
They may cost points to use.

The following table describes the stream commands.
Arguments are listed in the string too: `%command <argument1> <argument2>...`
`<argument?>` means an optional argument.

|command|description|cost|karma effect|
|---|---|---|---|
|`%checkin`|Check in to the stream. Can only be used once per overlay restart.|Free|NA|
|`%points <username?>`|Checks how much you have. If specified username, checks how much they have.|Free|NA|
|`%flashbang`|Deploying a flashbang|500|-100 karma|
|`%invest <amount>`|Invests `<amount>` to the stock market|`<amount>`|NA|
|`%uninvest <amount>`|Withdraw `<amount>` from the stock market|`<amount>`|NA|
|`%transfer <username> <amount>`|From your balance, gives `<username>` `<amount>` of points.|`<amount>`|NA|
|`%selfthought <message>`|Say something as if you were vanor. See [docs]({{< relref "overlay/selfthought.md" >}})|5000|-200|
|`%block <command>`|Blocks a command via a community bid.|NA|NA|
|`%unblock <command>`|Unblocks a command via a community bid.|NA|NA|
|`%kill <username>`|Kills a user.|NA|NA|


VIPs have an additional set of commands they can run.

|command|description|cost|
|---|---|---|
|`%poll <question>;<duration in seconds>;<option 1>;<option 2>;...;<option n>`|Start a poll|Free|
|`%endpoll`|Ends the current poll|Free|

## Standard Trinket Commands

These exist in a separate category because trinkets uses another system outside of overlays.
Trinkets can spawn randomly without prompting.
Trinkets do not cost any currency to use.

|command|description|karma effect|remark|
|---|---|---|---|
|`%rotate`|Rotates the screen|Consumes 100 Karma|Has a strict cooldown of 1800s and has a random chance of 0.001 from spawning from chat messages. |
|`%distract`|Spawns either first, second, third or fourth trumpet|Consumes 100 Karma|Has a strict cooldown of 300s and has a random cahnce of 0.01 from spawning from chat messages.|

Learn more about [trinkets]({{<relref "overlay/trinket.md" >}}).

## Standard Model Commands

These commands affect the model used by Vanor.

|command|description|karma effect|
|--|---|---|
|`%undress`|Undresses Vanor|Consumes and requires at least +50 Karma|
|`%hearts`|Gives Vanor some heart eyes|Consumes and requires at least +5 Karma|
|`%stars`|Gives Vanor some star eyes|Consumes and requires at least +5 Karma|

## VIP Overlay Commands

All VIPs are entitled to one stream command.
They will receive special treatment when they run the command, but normal chatters can also use them for a price.
The VIP entitlements are not stated (because they should know).

|command|description|VIP|normal cost|karma effect|
|---|---|---|---|---|
|`%blacksilence`|Does a bunch of silencing. Check [docs]({{ relref "overlay/blacksilence.md" }})|nikitakik228|500|50
|`%maxwell`|Spawn a bouncing spinning cats|5kuli|100|NA|
|`%showimage <url or tag> <tag?>`|Shows any image on the screen. If a url is provided, and a tag is provided thereafter, saves it. Requires approval from mod or mayoigo if URL.|mayoigo_QwQ|10000|-200|
|`%playaudio <url or tag> <tag?>`|Plays any audio. If a url is provided, and a tag is provided thereafter, saves it. Requires approval from mod or SpookiestSpooks if URL.|SpookiestSpooks|10000|-100|
|`%goodnightkiss`|Forces vanor to say goodnight to you to proceed with the stream. Also, times you out.|pastel8844|5000|-300|
|`%mistake`|a mistake|Mr_Auto|5000|-1000|
|`%settitle`|sets the title of the stream|sekatsu1|1000|**requires** 100 karma to execute. resultant karma will be `-0.3 * current karma value`, effectively flipping the karma.|
