---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Seiten‑Barcode‑Bereich dar, der verwendet wird, um einen Barcode‑Wert in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren."
type: docs
weight: 18
url: /de/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Stellt einen Seiten‑Barcode‑Bereich dar, der verwendet wird, um einen Barcode‑Wert in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getValue()](#getValue--) | Ruft den Barcode-Wert ab. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Ruft den Namen des Barcode-Typs ab. |
|
|  | [getConfidence()](#getConfidence--) | Ruft das Vertrauensniveau des geparsten Barcodes ab. |
|
|  | [getAngle()](#getAngle--) | Ruft den Winkel des Barcodes ab. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Der Wert des Barcodes. |
|
|  | codeTypeName | java.lang.String | Der Typname des Barcodes. |
|
|  | confidence | int | Das Vertrauensniveau des geparsten Barcodes. |
|
|  | angle | double | Der Winkel des Barcodes. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die den Barcode-Bereich enthält. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Barcode-Bereich enthält. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Ruft den Barcode-Wert ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der einen Wert des Barcode-Seitenbereichs darstellt.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Ruft den Namen des Barcode-Typs ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der einen Typnamen des Barcodes darstellt.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Ruft das Vertrauensniveau des geparsten Barcodes ab.


**Returns:**
int - Ein ganzzahliger Wert, der das Vertrauensniveau des geparsten Barcodes (0‑100) darstellt.

### getAngle() {#getAngle--}
```
public double getAngle()
```


Ruft den Winkel des Barcodes ab.


**Returns:**
double - Ein Gleitkommawert, der den Winkel des Barcodes (0‑360) darstellt.

