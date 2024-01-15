+++
title = "Player"
description = "Klasa gracza."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [CharacterBody2D](../CharacterBody2D)

## Description

Klasa gracza.

## Property Descriptions

### walking\_speed

```gdscript
@export var walking_speed: float = 600
```

Prędkość poruszania się.

### venting\_speed

```gdscript
@export var venting_speed: float = 1500
```

Prędkość teleportacji do venta.

### direction\_last\_x

```gdscript
var direction_last_x: float = -1
```

Ostatni kierunek poziomego ruchu gracza.

### can\_use\_vent

```gdscript
var can_use_vent: bool = false
```

Czy może używać venta.

### is\_in\_vent

```gdscript
var is_in_vent: bool = false
```

Czy jest w vencie.

### is\_moving\_through\_vent

```gdscript
var is_moving_through_vent: bool = false
```

Czy jest w trakcie poruszania się przez venta lub do venta.

### can\_report

```gdscript
var can_report: bool = false
```

Określa czy gracz może reportować

### is\_teleport

```gdscript
var is_teleport: bool = false
```

Czy jest w trakcie teleportacji.

### teleport\_position

```gdscript
var teleport_position = null
```

Pozycja docelowa teleportacji.

### input\_synchronizer

```gdscript
var input_synchronizer: InputSynchronizer
```

Referencja do wejścia gracza.

## Method Descriptions

### get\_nearest\_vent

```gdscript
func get_nearest_vent() -> Vent
```

Zwraca najbliższy vent.

### has\_vent\_permission

```gdscript
func has_vent_permission(vent: Vent) -> bool
```

Zwraca czy gracz może używać ventów.

### toggle\_visibility

```gdscript
func toggle_visibility(is_enabled: bool)
```

Zmienia widoczność gracza.

### closest\_player

```gdscript
func closest_player(to_who: int) -> int
```

Zwraca id: int najbliższego gracza do "to_who", który nie jest impostorem i żyje.

### activate\_lights

```gdscript
func activate_lights()
```

Włącza światło graczowi.

### deactivate\_lights

```gdscript
func deactivate_lights()
```

Wyłącza światło graczowi.

### activate\_player\_shaders

```gdscript
func activate_player_shaders()
```

Włącza shadery graczowi.

### deactivate\_player\_shaders

```gdscript
func deactivate_player_shaders()
```

Wyłącza shadery graczowi.

### set\_light\_texture\_scale

```gdscript
func set_light_texture_scale(texture_scale: float)
```

Ustawia wartość promienia światła graczowi.

### decrease\_light\_range\_sabotage

```gdscript
func decrease_light_range_sabotage() -> void
```

Zmniejsza promień swiatła podczas sabotażu.

### cancel\_decrease\_light\_range\_sabotage

```gdscript
func cancel_decrease_light_range_sabotage() -> void
```

Ustawia promień światła na normalny po sabotażu.

## Signals

- signal vent_entered(): Emitowany, gdy gracz wchodzi do venta.
- signal vent_exited(): Emitowany, gdy gracz wychodzi z venta.
- signal button_active(button_name, is_active): Emitowany, gdy przycisk powinien być włączony/wyłączony.
