+++
title = "PopUpWindow"
description = "Klasa okienka z informacją."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Control](../Control)

## Description

Klasa okienka z informacją.

## Property Descriptions

### one\_button

```gdscript
@export var one_button: bool = false
```

True - jedne przycisk, False - dwa przyciski.

### information

```gdscript
@export var information: String = "information"
```

Wyświetlana informacja.

### left\_button\_text

```gdscript
@export var left_button_text: String = "left"
```

Tekst na lewym przycisku.

### right\_button\_text

```gdscript
@export var right_button_text: String = "right"
```

Tekst na prawym przycisku.

### middle\_button\_text

```gdscript
@export var middle_button_text: String = "middle"
```

Tekst na środkowym przycisku.

## Method Descriptions

### set\_information

```gdscript
func set_information(text: String)
```

Ustawia wyświetlaną informacje.

## Signals

- signal left_pressed(): Emitowany po naciśnięciu przycisku z lewej strony.
- signal right_pressed(): Emitowany po naciśnięciu przycisku z prawej strony.
- signal middle_pressed(): Emitowany po naciśnięciu przycisku na środku.
