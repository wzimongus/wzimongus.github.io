+++
title = "ReportArea"
description = "Klasa obszaru raportowania."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Area2D](../Area2D)

## Description

Klasa obszaru raportowania.

## Property Descriptions

### is\_button

```gdscript
@export var is_button: bool = false
```

Określa czy jest przyciskiem.

### body\_texture

```gdscript
@export var body_texture: Texture
```

Tekstura znalezionego ciała.

## Signals

- signal button_active(button_name, is_active): Sygnał aktywujący/deaktywujący przyciski w interfejsie.
- signal toggle_button_highlight(is_active): Sygnał przełączający podświetlenie przycisku awaryjnego.
