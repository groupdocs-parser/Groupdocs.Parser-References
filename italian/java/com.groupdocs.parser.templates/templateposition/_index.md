---
title: "TemplatePosition"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce una classe astratta base per le posizioni del modello."
type: docs
weight: 18
url: /it/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Fornisce una classe astratta base per le posizioni del modello.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Crea una copia della posizione corrente con tutte le coordinate scalate del fattore fornito. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Crea una copia della posizione corrente con tutte le coordinate scalate del fattore fornito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | fattore | double | Il fattore di scala. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

