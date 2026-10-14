---
title: "TemplateOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für das Parsen mittels Vorlagenfunktionalität verwendet werden."
type: docs
weight: 17
url: /de/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Stellt die Optionen bereit, die für das Parsen mittels Vorlagenfunktionalität verwendet werden.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Initialisiert eine neue Instanz der [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Liefert die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Initialisiert eine neue Instanz der [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangleTolerance | double | Die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Liefert die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen.


**Returns:**
double - Der double-Wert von 0 (kein Rand) bis 1 (das gesamte Element ignorieren).

