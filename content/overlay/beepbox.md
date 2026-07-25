---
title: Beepbox
---

# Beepbox

Beepbox lets you play custom melodies on stream. It has three parts:

- A Discord bot (known as "SongBot")
- The `<songname>` chat syntax
- A spinning vanor visual on screen when a song plays

Beepbox comes from the [BeepBox](https://www.beepbox.co) site, where you can make custom melodies in your browser.

## Discord SongBot

SongBot lives in the **[#song](https://discord.com/channels/1324837719859396668/1330568746124709990)** channel on the vanor Discord server.

### Commands

|command|description|
|---|---|
|`/song save`|Save a new beepbox song. Attach a `.json` or `.beepbox` file with your command.|
|`/song list`|List all saved songs, with paginated navigation.|
|`/song delete`|Delete one of your songs, or any song if you are a moderator.|

To create a song, design your melody on [beepbox.co](https://www.beepbox.co), export the file, and attach it with `/song save`.

## Playing Songs

To play a saved song on stream, type the song name surrounded by angle brackets:

```
<songname>
```

This triggers the beepbox player on the overlay, showing a spinning vanor visual.
Playing songs is free.

> [!IMPORTANT]
> **TODO**: add screenshots of the Discord bot interface and the spinning vanor overlay.
