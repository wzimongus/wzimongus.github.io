+++
title = "VotingScreenPlayerBox"
description = "Klasa odpowiadająca za box gracza w ekranie głosowania."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Control](../Control)

## Description

Klasa odpowiadająca za box gracza w ekranie głosowania.

## Method Descriptions

### init

```gdscript
func init(player_id: int, voted_by: Array)
```

Funkcja inicjalizująca box gracza.

### set\_voting\_status

```gdscript
func set_voting_status(is_voted: bool)
```

Funkcja ustawiająca status głosowania.

## Signals

- signal player_voted(): Sygnał emitowany gdy gracz zagłosuje.
- signal player_selected(): Sygnał emitowany gdy gracz zostanie wybrany.
