---
title: "%check"
---

# %check

The `%check` command evaluates the success and failure chances of another command without executing it. You can use it to preview odds before spending points, particularly useful for [stock market]({{< relref "stock.md" >}}) buys.

## Usage

```
%check <%command> [args...]
```

Provide the full command invocation you want to inspect. For example:

```
%check %buy HEART 100
%check %buy HEART 50 20
%check %gamba 500
```

## How It Works

`%check` computes two layers of chance:

1. **Gate chance**: The standard command-level success probability, factoring in your subscription tier and bit bonuses.
2. **Inner chance** (optional): A command-specific evaluation. For `%buy`, this simulates the stock market buy to show the actual fail probability without deducting points or creating holdings.

The reply shows both percentages and the timeout duration you would face on failure. If the inner evaluation fails (e.g. not enough check-ins), the error is shown instead.

## Supported Commands

Currently, `%buy` is the only command with a command-specific inner evaluation. For all other commands, only the gate chance is computed.

Broadcasters are gently mocked for using the command, because the chances would be the same for them anyway.
