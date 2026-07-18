---
weight: 10
title: "Stream Commands"
---

# Stream Commands

## StreamElement Commands

No stream effect. Information or mod commands.

- `!discord` -- Discord invite
- `!sfx` -- Sound effect list
- `!piss` -- Piss copypasta
- `!docs` -- Docs copypasta

## Standard Overlay Commands

Everyone can use these. Some cost [points]({{<relref "overlay/points.md" >}}).

`<argument?>` = optional.

|command|description|cost|karma|
|---|---|---|---|
|`%checkin`|Check into stream. Once per overlay restart.|Free|NA|
|`%points <username?>`|Your points, or another user's.|Free|NA|
|`%flashbang`|Flashbang on screen.|500|-100|
|`%buy <stock> <amount> <price>`|Place a buy order on the [stock market]({{<relref "overlay/stock.md" >}}).|`<amount>*<price>`|NA|
|`%sell <stock> <amount> <price>`|Place a sell order on the stock market.|`<amount>*<price>`|NA|
|`%stocks`|Check your portfolio and open orders.|Free|NA|
|`%buyorders`|See random buy orders on the book.|Free|NA|
|`%sellorders`|See random sell orders on the book.|Free|NA|
|`%gamba`|Gamble spin. 60s cooldown.|Free|NA|
|`%transfer <username> <amount>`|Give points to another user.|`<amount>`|NA|
|`%selfthought <message>`|Speak as robo-vanor. 5000 cost.|5000|-200|
|`%block <command>`|Community bid to block a command.|NA|NA|
|`%unblock <command>`|Community bid to unblock.|NA|NA|
|`%kill <username>`|Kill a user.|NA|NA|

### VIP extras

|command|description|cost|
|---|---|---|---|
|`%poll <q>;<sec>;<o1>;<o2>;...`|Start a poll.|Free|
|`%endpoll`|End current poll.|Free|
|`%prediction <title>;<durationSec>;<option1>;<option2>;...`|Create a Twitch prediction.|10000|
|`%endprediction`|Lock and resolve the current prediction.|Free|
|`%endstream`|Close stock market and pay out holdings. Broadcaster only.|Free|

## Standard Trinket Commands

Use a separate system. Can trigger randomly. No point cost.

|command|description|karma|cooldown|spawn chance|
|---|---|---|---|---|
|`%rotate`|Rotates the screen.|-100|1800s|0.001|
|`%distract`|Spawns a trumpet.|-100|300s|0.01|

More at [trinkets]({{<relref "overlay/trinket.md" >}}).

## Standard Model Commands

Affect vanor's model.

|command|description|karma|
|---|---|---|
|`%undress`|Undress vanor.|Requires >= +50|
|`%hearts`|Heart eyes.|Requires >= +5|
|`%stars`|Star eyes.|Requires >= +5|

## VIP Overlay Commands

Each VIP gets one exclusive command. Normal chatters can use them too for a price.

|command|description|VIP|normal cost|karma|
|---|---|---|---|---|
|`%blacksilence`|Silence everything. See [docs]({{< relref "overlay/blacksilence.md" >}}).|nikitakik228|500|50|
|`%maxwell`|Bouncing spinning cat.|5kuli|100|NA|
|`%showimage <url> <tag?>`|Show image on screen. URL+tag saves it. Needs mod/mayoigo_QwQ approval.|mayoigo_QwQ|10000|-200|
|`%playaudio <url> <tag?>`|Play audio. URL+tag saves it. Needs mod/SpookiestSpooks approval.|SpookiestSpooks|10000|-100|
|`%goodnightkiss`|Goodnight timeout.|pastel8844|5000|-300|
|`%mistake`|A mistake.|Mr_Auto|5000|-1000|
|`%settitle`|Set stream title.|sekatsu1|1000|Requires 100. Result: -0.3x current karma.|
