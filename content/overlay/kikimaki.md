---
title: Kiki and Maki
---

# Kiki and Maki

Kiki and Maki are AI cats that appear on the stream in different forms.

## Kiki

Kiki is a small fine-tuned LLM that runs on a cloud server (Modal GPU).

She sometimes responds to chat messages with [kaomoji](https://en.wikipedia.org/wiki/Kaomoji) and emoji reactions. These appear directly below [chat bullets]({{< relref "bullet.md" >}}).

To directly interact with Kiki, include the word "kiki" anywhere in your message.
Otherwise, she has a small chance of reacting to random messages.

Kiki also issues [karma]({{< relref "karma.md" >}}) ratings for messages she reacts to. The scale goes from **-500 to +50**.
She can also mark messages as "pin-worthy." Pinned messages may appear on the overlay.

## Maki

Maki is a much larger system that combines speech-to-text, an LLM via [OpenRouter](https://openrouter.ai), and several tools.

She runs on vanor's local machine and can only hear vanor. There is currently no way for chat to interact with her directly.
Her responses appear as overlay popups.

### Activation

Maki has two trigger modes:

- **Voice activation (VAD)**: Maki listens for a wakeword via microphone. When detected, she captures a voice utterance and processes it.
- **Autonomous**: about every 15 minutes at random, Maki wakes up on her own. She takes a screenshot, reads recent chat, and decides whether to act.

### What Maki Can Do

Maki has tools to interact with the stream:

- Read and respond to recent chat messages
- Change the stream title
- Create Twitch polls
- Timeout users
- Send messages as vanor (`%selfthought`)
- Trigger other chat commands (`%blacksilence`, `%maxwell`, `%distract`, `%rotate`, `%goodnightkiss clear`, `%mistake`, `%grayscale`)
- Take screenshots for visual context
- Search the web
- Generate and save code
- Use deep reasoning for complex tasks (via a separate LLM)

Maki uses different AI models for different jobs. A main model handles conversation. A separate evaluator model handles code generation. A deep reasoning model handles multi-step analysis.

### Screenshots

Maki captures the screen for visual context. While she takes a screenshot, the overlay hides itself for a moment so the capture is clean.
