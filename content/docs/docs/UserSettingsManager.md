+++
title = "UserSettingsManager"
description = "Klasa odpowiadająca za zapis ustawień gracza."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Resource](../Resource)

## Description

Klasa odpowiadająca za zapis ustawień gracza.

## Property Descriptions

### volume

```gdscript
@export var volume: int = 20
```

Ustawienia dźwięku, początkowo ustawione na domyślne.

### interface\_scale

```gdscript
@export var interface_scale: float = 1
```

Ustawienia skali interfejsu, początkowo ustawione na domyślne.

### full\_screen

```gdscript
@export var full_screen: bool = false
```

Ustawienia pełnego ekranu, początkowo ustawione na domyślne.

### v\_sync

```gdscript
@export var v_sync: bool = true
```

Ustawienia v-sync, początkowo ustawione na domyślne.

### controls\_dictionary

```gdscript
@export var controls_dictionary
```

Ustawienia sterowania, początkowo ustawione na domyślne.

## Method Descriptions

### save

```gdscript
func save()
```

Zapisuje ustawienia.

### restore\_default\_sound\_and\_graphics

```gdscript
func restore_default_sound_and_graphics()
```

Przywraca domyślne ustawienia dźwięku i grafiki.

### restore\_default\_controls

```gdscript
func restore_default_controls()
```

Przywraca domyślne ustawienia sterowania.

### change\_interface\_scale

```gdscript
func change_interface_scale(value: float)
```

Zmienia skalę interfejsu.

### load\_or\_create <small>(static)</small>

```gdscript
func load_or_create()
```

Zwraca zapisane ustawienia z pliku lub tworzy nowy plik z domyślnymi ustawieniami i je zwraca.

## Signals

- signal interface_scale_value_changed(value): Emitowany po zmianie skali interfejsu.
