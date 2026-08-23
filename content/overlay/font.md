---
title: "Font"
---

# Font

The `%font` command changes the font used for your [chat bullets]({{< relref "bullet.md" >}}), covering both your username and your message text.

- `%font <fontname>` - uses the font named `<fontname>`
- `%font default` or `%font reset` - goes back to the default font

If the font name doesn't exist, the command tells you to check `/font list` in Discord.

It is sqbika's VIP command, costing **10000 points** when used by non-VIP chatters.

## Font Weight & Italics

Two additional commands change the styling of your [chat bullet]({{< relref "bullet.md" >}}) text:

- `%fontweight <bold|normal>` - makes your username and message text bold or normal
- `%fontitalic <on|off>` - turns italics on or off

Both are sqbika's VIP commands, also costing **10000 points** for non-VIP chatters, and persist across streams like `%font`.

## Fonts

Fonts are managed in the Discord font channel:

- `/font submit <fontname> <fontfile>` - submits a font for approval, with a preview for approvers
- `/font list [page]` - lists all registered fonts

Font files must be `.woff2`, `.woff`, `.ttf`, `.otf` or `.svg` and at most 1MB. Font names are lowercase, max 32 characters, and limited to letters, numbers, `_` and `-`.

`%font` only accepts fonts that are already registered.
