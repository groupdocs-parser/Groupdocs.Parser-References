---
title: "TemplatePosition"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine abstrakte Basisklasse für Vorlagenpositionen bereit."
type: docs
weight: 18
url: /de/java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Stellt eine abstrakte Basisklasse für Vorlagenpositionen bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Erstellt eine Kopie der aktuellen Position, wobei alle Koordinaten um den angegebenen Faktor skaliert werden. |
|
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Erstellt eine Kopie der aktuellen Position, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Faktor | double | Der Skalierungsfaktor. |
|

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.

