+++
title = "SettingsKeyRebind"
description = "Klasa obsługująca przypisanie przycisków do akcji."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Control](../Control)

## Description

Klasa obsługująca przypisanie przycisków do akcji.

## Property Descriptions

### action\_label\_name

```gdscript
@export var action_label_name: String = "_action name"
```

Nazwa akcji dla etykiety.

### action\_project\_name

```gdscript
@export var action_project_name: String
```

Nazwa akcji w ustawieniach projektu.

## Method Descriptions

### start

```gdscript
func start()
```

Obsługuje przypisanie przycisków i ustawienie nazw etykiet i nazw przycisków.

## Signals

- signal rebind_button_pressed(action_label_name, action_project_name, side, left_button, right_button): Emitowany po naciśnięciu przycisku.
