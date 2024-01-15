+++
title = "Chat"
description = "Klasa czatu."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [CanvasLayer](../CanvasLayer)

## Description

Klasa czatu.

## Constants Descriptions

### FADE\_OUT\_TIME

```gdscript
const FADE_OUT_TIME: float = 0.25
```

Czas po którym czat zniknie

### GROUP\_COLORS

```gdscript
const GROUP_COLORS: Dictionary = {"0":"white","1":"red","2":"gray","3":"yellow"}
```

Kolor grupy

### Group

```gdscript
enum Group{GLOBAL = 0, LECTURER = 1, DEAD = 2, SYSTEM = 3}
```

Grupy czatu

## Method Descriptions

### send\_system\_message

```gdscript
func send_system_message(message)
```

Wysyła wiadomość systemową.

### open\_chat

```gdscript
func open_chat()
```

Otwiera czat.

### close\_chat

```gdscript
func close_chat()
```

Zamyka czat.

## Signals

- signal input_visibility_changed(): Emitowany, gdy zmieni się widoczność pola tekstowego.
