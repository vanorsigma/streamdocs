---
title: "Model"
---

# Model

Vanor's VTuber model is controlled by several systems.

{{< figure src="/vanorBlush.png" title="Vanor Blushing" >}}

## Heart Rate Effects

The model's expression is affected by vanor's heart rate, which is tracked in real time:

|threshold|effect|
|---|---|
|>= 80 BPM|Blush mode active|
|<= 50 BPM|Despair mode active|

The heart rate also drives the [stock market]({{< relref "overlay/stock.md" >}}), creating a feedback loop between vanor's physical state and in-stream mechanics.

## Model Blendshapes

Chatters can toggle model blend shapes using the [standard model commands]({{< relref "commands.md#standard-model-commands" >}}):

- `%hearts` gives heart eyes (5 karma)
- `%stars` gives star eyes (5 karma)
- `%undress` undresses the model (50 karma)

Each toggle lasts for 60 seconds before automatically reverting.
