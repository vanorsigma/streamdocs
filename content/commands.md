---
weight: 10
title: "Stream Commands"
---

# Stream Commands

There are several kinds of commands, each affecting different parts of the stream.

## StreamElements Commands

These have no effect on the stream overlay, and are usually either mod commands or commands displaying information.

- `!discord` - Shows the Discord invite link
- `!sfx` - Shows a list of available sound effects
- `!piss` - The piss copypasta
- `!docs` - The docs copypasta

## Standard Overlay Commands

These are commands everyone can run. Most cost points to use.

Arguments are listed in the command string: `%command <argument1> <argument2>...`
`<argument?>` means an optional argument.

|command|description|cost|karma effect|
|---|---|---|---|
|`%checkin` / `%chicken`|Check in to the stream. Can only be used once per overlay restart. Awards 1000 points.|Free|NA|
|`%points <username?>`|Checks your points balance. If a username is provided, checks theirs.|Free|NA|
|`%transfer <username> <amount>`|Transfers `<amount>` of your points to `<username>`.|`<amount>`|NA|
|`%flashbang`|Deploys a flashbang on the screen.|500|-100 karma|
|`%buy <symbol> <amount> [overpay]`|Invest `<amount>` points in a stock. Use `all` for your full balance. See [Stock Market]({{< relref "overlay/stock.md" >}}).|`<amount>`|NA|
|`%sell <symbol> <amount>`|Withdraw `<amount>` from your stock holdings. Use `all` to sell everything.|`<amount>`|NA|
|`%stocks`|View your current stock portfolio.|Free|NA|
|`%gamba <amount>`|Spin the [gamba wheel]({{< relref "overlay/gamba.md" >}}). Random outcomes range from free points to timeouts.|`<amount>`|NA|
|`%selfthought <message>`|Say something as if you were vanor. See [Self-thought]({{< relref "overlay/selfthought.md" >}}).|5000|-200|
|`%grayscale`|Applies a grayscale shader to the screen for 2 minutes.|1000|-100|
|`%bid`|Start or contribute to a community bid.|Varies|NA|
|`%endbid`|End an active community bid.|Free|NA|
|`%refreshVoice`|Reroll your TTS voice. See [TTS]({{< relref "overlay/TTS.md" >}}).|Free|NA|

## Standard Trinket Commands

These exist in a separate category because trinkets use another system outside of overlays.
Trinkets can also spawn randomly without prompting.
Trinkets do not cost points, but consume karma.

|command|description|karma effect|remark|
|---|---|---|---|
|`%rotate`|Rotates vanor's screen.|Consumes 100 karma|1800s cooldown. Has a 0.1% random chance of triggering from chat messages.|
|`%distract`|Spawns a random distraction: emote guessing, song guessing, or a boss fight. See [Trinkets]({{< relref "overlay/trinket.md" >}}).|Consumes 200 karma|300s cooldown. Has a 1% random chance of triggering from chat messages.|

Learn more about [trinkets]({{< relref "overlay/trinket.md" >}}).

## Standard Model Commands

These commands affect the model used by vanor.

|command|description|karma effect|duration|
|---|---|---|---|
|`%undress`|Undresses vanor's model.|Consumes and requires at least +50 karma|60s|
|`%hearts`|Gives vanor heart eyes.|Consumes and requires at least +5 karma|60s|
|`%stars`|Gives vanor star eyes.|Consumes and requires at least +5 karma|60s|

## VIP Overlay Commands

All VIPs are entitled to one stream command.
They receive free usage of their command, while normal chatters can also use them for a cost.
The VIP entitlements are not stated (because they should know).

|command|description|VIP|normal cost|karma effect|
|---|---|---|---|---|
|`%blacksilence`|Silences TTS, clears chat bullets, cancels trinkets and beepbox songs. See [Black Silence]({{< relref "overlay/blacksilence.md" >}}).|nikitakik228|500|+50|
|`%maxwell`|Spawns bouncing spinning Maxwell bread cats on the screen.|5kuli|100|NA|
|`%showimage <url or tag> <tag?>`|Shows any image on the screen. If a URL is provided with a tag, saves it for future use. External URLs require approval from a moderator or mayoigo.|mayoigo_QwQ|1000|-200|
|`%playaudio <url or tag> <tag?>`|Plays any audio. If a URL is provided with a tag, saves it for future use. External URLs require approval from a moderator or SpookiestSpooks.|SpookiestSpooks|5000|-100|
|`%goodnightkiss`|Overlays a goodnight kiss animation and times you out for 30 minutes.|pastel8844|200|-300|
|`%mistake`|Increments the mistake counter.|Mr_Auto|500|-1000|
|`%settitle <newTitle>`|Changes the stream title. Requires at least 100 karma to execute.|sekatsu1|1000|Modifier: -0.3× current karma|
|`%poll <title>;<duration>;<opt1>;<opt2>;[opt3;[opt4;[opt5]]]`|Creates a Twitch poll. Semicolon-delimited. Duration in seconds (15-1800). 2-5 options.|NA|Free|NA|
|`%endpoll`|Ends the current Twitch poll.|NA|Free|NA|
|`%prediction <title>;<duration>;<opt1>;<opt2>`|Creates a Twitch prediction with exactly 2 outcomes. Duration in seconds (15-1800).|NA|Free|NA|
|`%endprediction`|Ends the active Twitch prediction.|NA|Free|NA|

## Mod Commands

These commands are available to moderators and affect chat-wide systems.
See [Moderation]({{< relref "overlay/moderation.md" >}}) for more details.

|command|description|cost|karma effect|
|---|---|---|---|
|`%block <command>`|Blocks a command by starting a community bid. Minimum bid: 1000 points.|NA|NA|
|`%unblock <command>`|Unblocks a command by starting a community bid. Minimum bid: 1000 points.|NA|NA|
|`%kill <username>`|Starts a community vote to timeout a user. Vote target: 2000 points.|NA|NA|
|`%resetcooldown [username\|all]`|Resets command cooldowns. Without argument resets your own cooldowns. `all` resets all overlay cooldowns (mod only).|Free (self), 20000 (other)|NA|
