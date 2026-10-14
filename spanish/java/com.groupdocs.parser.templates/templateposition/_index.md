---
title: "TemplatePosition"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona una clase abstracta base para las posiciones de plantilla."
type: docs
weight: 18
url: /es/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Proporciona una clase abstracta base para las posiciones de plantilla.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Crea una copia de la posición actual con todas las coordenadas escaladas por el factor dado. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Crea una copia de la posición actual con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | factor | double | El factor de escala. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

