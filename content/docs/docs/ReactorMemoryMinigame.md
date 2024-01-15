+++
title = "ReactorMemoryMinigame"
description = "Klasa reprezentująca instancję gry Reactor Memory Answer."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Description

Klasa reprezentująca instancję gry Reactor Memory Answer.

## Property Descriptions

### polish\_name

```gdscript
@export var polish_name: String
```

Polska nazwa minigry.

### flash\_length

```gdscript
var flash_length = 0.5
```

Czas trwania błysku.

### flash\_pause

```gdscript
var flash_pause = 0.1
```

Czas trwania przerwy między błyskami.

## Method Descriptions

### player\_pressed

```gdscript
func player_pressed(name)
```

Funkcja wywoływana po naciśnięciu przycisku przez gracza.

## Signals

- signal minigame_end(): Emitowany, gdy minigra zostanie ukończona.
