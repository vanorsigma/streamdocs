---
title: TTS
---

# TTS

By default, your chat message will be read aloud by the TTS system for free.

The TTS system randomly assigns you a voice each time, along with a pop-cat overlay on the screen.
To reroll your voice, use `%refreshVoice`.

## Modifiers

You can control how your message is spoken with inline modifiers:

- `[fast]` speeds up the speech
- `[slow]` slows down the speech
- `[high]` raises the pitch
- `[low]` lowers the pitch

Example:
```
[fast] i am [slow] really [high] cool
```

Modifiers can be placed anywhere in your message and affect the text that follows.

TODO insert screenshot of TTS overlay with pop-cat

## Sound Effects

The TTS system also supports sound effects triggered inline.
Wrap a sound effect tag in parentheses:

```
here, have some metal pipes. (metalpipes)
```

The full list of available sound effects can be found with `!sfx` in chat.

Sound effects play at the same time as your TTS message. They don't interrupt speech.

## Filtering

Some messages are filtered out and will not be read by TTS:

- Messages starting with `!`, `` ` ``, `~`, or `{`
- URLs
- Messages over 200 characters
- Messages consisting mostly of numbers (7+ digits)
- Certain banned phrases and copypasta

## Black Silence

The `%blacksilence` command temporarily disables all TTS output and clears the current TTS queue.
See [Black Silence]({{< relref "blacksilence.md" >}}) for details.
