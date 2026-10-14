---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion von Seitenbereichen verwendet werden."
type: docs
weight: 28
url: /de/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Stellt die Optionen bereit, die für die Extraktion von Seitenbereichen verwendet werden.

Eine Instanz der Klasse [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) wird als Parameter in [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-) verwendet.
und den Methoden [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) mit der Größe des zu ignorierenden Randes. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Initialisiert eine neue Instanz der Klasse [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Liefert das rechteckige Gebiet, das Seitenbereiche enthält. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Liefert die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) mit der Größe des zu ignorierenden Randes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das rechteckige Gebiet, das Seitenbereiche enthält. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Initialisiert eine neue Instanz der Klasse [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das rechteckige Gebiet, das Seitenbereiche enthält. |
|
|  | rectangleTolerance | double | Die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Liefert das rechteckige Gebiet, das Seitenbereiche enthält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Liefert die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen.


**Returns:**
double - Der double-Wert von 0 (kein Rand) bis 1 (das gesamte Element ignorieren).

