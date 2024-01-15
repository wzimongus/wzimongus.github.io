+++
title = "EmergencyButton"
description = "Klasa przycisku awaryjnego spotkania."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Description

Klasa przycisku awaryjnego spotkania.

## Method Descriptions

### handle\_report

```gdscript
func handle_report(is_button: bool, body_id)
```

Obsługuje report/zebranie awaryjne.

## Signals

- signal emergency_timer_timeout(is_over): Emitowany, gdy zakończy się czas oczekiwania na aktywację przycisku.
- signal button_active(button_name, is_active): Emitowany, gdy przycisk interfejsu ma być aktywowany/deaktywowany.
