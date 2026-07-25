---
title: Trinkets (distract and rotate)
---

# Trinkets

"Trinkets" is the system behind `%rotate` and `%distract`. They spawn blocking overlays on vanor's screen.
They run in a separate desktop application (Trinket, built with PyQt6) outside of the browser overlay.

Trinkets do not cost points to use, but consume karma and have very long cooldowns.
They can also trigger randomly without using the commands. Each chat message has a small chance of triggering one.

## Rotate

`%rotate` captures a screenshot of the screen and rotates it continuously.
It has a **1800s cooldown** (30 minutes) and a **0.1% random chance** of triggering from chat.
Consumes **100 karma**.

## Distract

`%distract` spawns a random distraction from a set of mini-games.
It has a **300s cooldown** (5 minutes) and a **1% random chance** of triggering from chat.
Consumes **200 karma**.

When triggered, the distraction appears as a warning frame (inspired by Lobotomy Corporation) with one of four threat levels.
The distraction types are:

- **Emote guessing**: a random 7TV emote is displayed. Type its name to dismiss it.
- **Song guessing**: a random song plays from the trinket song library. Guess the title to dismiss it.
- **Boss fight**: a boss appears on screen with four emotes. Chatters must type the correct emote name to deal damage. The boss moves around the screen and has a health bar.

Multiple distraction windows can appear at once. The warning frame closes when all child windows are dismissed.

Press **Escape** to dismiss the warning frame early.

TODO insert screenshots of the warning frame, emote guess, song guess, and boss fight

## Cancelling

Trinkets can be cancelled by `%blacksilence` or by the trinket `cancel` command from the overlay.
