---
title: "TemplatePosition"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller en abstrakt basklass för mallpositioner."
type: docs
weight: 18
url: /sv/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Tillhandahåller en abstrakt basklass för mallpositioner.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Skapar en kopia av den aktuella positionen med alla koordinater skalade med den angivna faktorn. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Skapar en kopia av den aktuella positionen med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | faktor | double | Skalfaktorn. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

