+++
title = "TaskButton"
description = "Klasa punktu interakcji z zadaniem."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Area2D](../Area2D)

## Description

Klasa punktu interakcji z zadaniem.

## Property Descriptions

### sprite

```gdscript
@export var sprite: Texture2D
```

Sprite wykorzystany jako przycisk zadania.

### scale\_factor

```gdscript
@export var scale_factor: float = 1
```

Współczynnik skalowania sprite'a zadania.

### task\_id

```gdscript
@export var task_id: int
```

Task ID przekazany przez serwer

### disabled

```gdscript
@export var disabled = true
```

Określa dostępność taska graczowi.

### is\_minigame

```gdscript
@export var is_minigame = true
```

Określa, czy punkt interakcji zawiera w sobie minigrę.

### minigame\_scene

```gdscript
@export var minigame_scene: PackedScene
```

Scena minigry która będzie włączona przez ten przycisk.

## Method Descriptions

### enable\_task

```gdscript
func enable_task(server_task_id)
```

Udostępnia punkt interakcji graczowi.

### disable\_task

```gdscript
func disable_task()
```

Zamyka dostęp do punktu interakcji.