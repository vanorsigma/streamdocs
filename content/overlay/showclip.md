---
title: "%showclip"
---

# %showclip

The `%showclip` command (`%sc` for short) plays a Twitch clip on the overlay. It disappears on its own once the clip ends.

```
%showclip https://clips.twitch.tv/SomeClipSlug
%showclip SomeClipSlug
```

Both a full Twitch clip URL and a bare clip ID work. The clip must be from vanor's own channel; clips from other channels are rejected.

It costs **15000 points** and has a 30-second cooldown. It is free for vanorsigma.

The overlay tags the clip with who clipped it (`clipped by <username>`).

Want to clip something yourself? See [`%clip`]({{< relref "clip.md" >}}).
