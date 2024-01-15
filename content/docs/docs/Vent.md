+++
title = "Vent"
description = "Klasa venta."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Description

Klasa venta.

## Property Descriptions

### vent\_target\_list

```gdscript
@export var vent_target_list: Array[Vent]
```

Lista docelowych ventów.

### direction\_button\_distance

```gdscript
@export var direction_button_distance: int = 60
```

Dystans przycisku kierunkowego od venta.

### allow\_student\_venting

```gdscript
@export var allow_student_venting: bool = false
```

Czy student może użyć venta.

## Method Descriptions

### set\_direction\_buttons\_visibility

```gdscript
func set_direction_buttons_visibility(visibility: bool)
```

Ustawia widoczność przycisków kierunkowych.

### set\_vent\_light\_visibility\_for

```gdscript
func set_vent_light_visibility_for(player_id: int, visibility: bool)
```

Włącza światło venta kiedy gracz znajduje się wewnątrz.

### play\_vent\_animation

```gdscript
func play_vent_animation()
```

Odtwarza animację ventowania.

## Signals

- signal vent_button_active(button_name, is_active): Emitowany gdy przycisk ventowania powinien być włączony/wyłączony.
