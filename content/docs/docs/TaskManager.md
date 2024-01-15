+++
title = "TaskManager"
description = "Klasa systemu zarządzania zadaniami w grze."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node](../Node)

## Description

Klasa systemu zarządzania zadaniami w grze.

## Property Descriptions

### current\_task\_id

```gdscript
var current_task_id = null
```

Task ID bieżącego zadania.

### current\_player\_tasks

```gdscript
var current_player_tasks
```

Przechowuje zadania bieżącego gracza.

### global\_tasks\_amount

```gdscript
var global_tasks_amount: int
```

Ilość zadań w całej grze.

### global\_tasks\_completed\_amount

```gdscript
var global_tasks_completed_amount: int
```

Ilość zrobionych już zadań.

## Method Descriptions

### assign\_tasks

```gdscript
func assign_tasks(task_amount)
```

Przypisuje zadania graczom.

### mark\_task\_as\_complete

```gdscript
func mark_task_as_complete() -> void
```

Oznacza zadanie jako wykonane po stronie klienta.

### set\_global\_tasks\_amount

```gdscript
func set_global_tasks_amount(amount: int) -> void
```

Ustawia początkową ilość zadań.

### remove\_player\_tasks

```gdscript
func remove_player_tasks(player_id: int)
```

Usuwa wszystkie zadania przypisane do tego gracza na serwerowej liście zadań.

### reset

```gdscript
func reset()
```

Resetuje zadania.

### get\_tasks\_server

```gdscript
func get_tasks_server()
```

Zwraca słownik wszystkich niezakończonych zadań przypisanych do wszystkich graczy.

## Signals

- signal tasks_change(): Emitowany kiedy lista zadań podlega zmianie.
- signal global_tasks_completed_amount_change(): Emitowany kiedy globalna lista zadań zostaje zmieniona.
