+++
title = "FillFormulasMinigame"
description = "Klasa reprezuntuje instancję minigry Fill Formulas."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Description

Klasa reprezuntuje instancję minigry Fill Formulas.

## Constants Descriptions

### FORMULAS

```gdscript
const FORMULAS: Dictionary = {"0":"F=m*v","1":"v=s/t","2":"a=v/t","3":"P=a²","4":"P=a*h","5":"P=π*r²","6":"P=a*h½"}
```

Lista możliwych do wylosowania wzorów

## Property Descriptions

### polish\_name

```gdscript
@export var polish_name: String
```

Polska nazwa minigry.

### how\_many\_formulas

```gdscript
@export var how_many_formulas = 3
```

Ilość losowanych wzorów

### is\_moving

```gdscript
var is_moving = false
```

Informacja czy pole jest obecnie przesuwane.

### moving

```gdscript
var moving
```

Referencja do przesuwanego pola.

### generated

```gdscript
var generated
```

Wcześniej wylosowane wzory.

## Signals

- signal minigame_end(): Emitowany, gdy minigra zostanie ukończona.
