---
title: "TemplatePosition"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt een abstracte basisklasse voor sjabloonposities."
type: docs
weight: 18
url: /nl/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Biedt een abstracte basisklasse voor sjabloonposities.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Maakt een kopie van de huidige positie waarbij alle coördinaten worden geschaald met de opgegeven factor. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Maakt een kopie van de huidige positie waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | factor | double | De schaalfactor. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

