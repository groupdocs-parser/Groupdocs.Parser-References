---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt das Vorlagen-Barcode-Feld bereit."
type: docs
weight: 11
url: /de/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Stellt das Vorlagen-Barcode-Feld bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Initialisiert eine neue Instanz der [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) Klasse mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Liefert den rechteckigen Bereich, der das Vorlagen-Barcode-Feld enthält. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Vorlagen-Barcode-Feld enthält. |
|
|  | Name | java.lang.String | Der Name des Barcode-Feldes. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Initialisiert eine neue Instanz der [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) Klasse mit dem GROSSBUCHSTABEN-Namen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Vorlagen-Barcode-Feld enthält. |
|
|  | Name | java.lang.String | Der Name des Barcode-Feldes. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) mit dem GROSSBUCHSTABEN-Namen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Vorlagen-Barcode-Feld enthält. |
|
|  | Name | java.lang.String | Der Name des Barcode-Feldes. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Vorlagen-Barcode-Feld enthält. |
|
|  | Name | java.lang.String | Der Name des Barcode-Feldes. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der das Vorlagen-Barcode-Feld enthält. |
|
|  | Name | java.lang.String | Der Name des Barcode-Feldes. |
|
|  | pageIndex | java.lang.Integer | Ein ganzzahliger Wert, der den Index der Seite darstellt, auf der das Vorlagenelement gefunden wird;  null  falls das Vorlagenelement auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Liefert den rechteckigen Bereich, der das Vorlagen-Barcode-Feld enthält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Erstellt eine Kopie des aktuellen Elements, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
