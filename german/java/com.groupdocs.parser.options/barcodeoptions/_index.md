---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Barcode‑Extraktion verwendet werden."
type: docs
weight: 10
url: /de/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Stellt die Optionen bereit, die für die Barcode‑Extraktion verwendet werden.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Initialisiert eine neue Instanz der BarcodeOptions-Klasse mit Standardwerten. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse BarcodeOptions mit dem rechteckigen Bereich. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Initialisiert eine neue Instanz der Klasse BarcodeOptions mit Qualitätseinstellungen und Code-Typen. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Initialisiert eine neue Instanz der Klasse BarcodeOptions. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Ruft den Wert ab, der angibt, ob falsche Barcodes erlaubt sind. |
|
|  | [getDimension()](#getDimension--) | Ruft die minimale Größe des minimalen Barcode-Elements ab. |
|
|  | [getImageQuality()](#getImageQuality--) | Ruft die Qualität eines Quellbildes ab. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Ruft die Qualität eines Quell-Barcodes ab. |
|
|  | [getRectangle()](#getRectangle--) | Liefert das rechteckige Gebiet, das Seitenbereiche enthält. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Ruft die Typen der zu lesenden Barcodes ab. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Setzt den Wert, der angibt, ob falsche Barcodes erlaubt sind. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Setzt die minimale Größe des minimalen Barcode-Elements. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Setzt die Qualität eines Quellbildes. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Setzt die Qualität eines Quell-Barcodes. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Setzt den rechteckigen Bereich, der Barcodes enthält. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Setzt die Typen der zu lesenden Barcodes. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Initialisiert eine neue Instanz der BarcodeOptions-Klasse mit Standardwerten.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse BarcodeOptions mit dem rechteckigen Bereich.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der Barcodes enthält. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Initialisiert eine neue Instanz der Klasse BarcodeOptions mit Qualitätseinstellungen und Code-Typen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Die Qualität eines Quellbildes. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Die Qualität eines Quell-Barcodes. |
|
|  | codeTypes | java.lang.String[] | Die Typen der zu lesenden Barcodes. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Initialisiert eine neue Instanz der Klasse BarcodeOptions.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der Barcodes enthält. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Die Qualität eines Quellbildes. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Die Qualität eines Quell-Barcodes. |
|
|  | dimension | java.lang.Float | Die minimale Größe des minimalen Barcode-Elements. |
|
|  | allowIncorrectBarcodes | boolean | Der Wert, der angibt, ob falsche Barcodes erlaubt sind. |
|
|  | codeTypes | java.lang.String[] | Die Typen der zu lesenden Barcodes. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Ruft den Wert ab, der angibt, ob falsche Barcodes erlaubt sind.


**Returns:**
boolean -  true  wenn falsche Barcodes erlaubt sind; andernfalls  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Ruft die minimale Größe des minimalen Barcode-Elements ab.


**Returns:**
java.lang.Float - Der Float-Wert, der das minimale Barcode-Element darstellt;  null  wenn der Automatikmodus verwendet wird.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Ruft die Qualität eines Quellbildes ab.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Ruft die Qualität eines Quell-Barcodes ab.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Liefert das rechteckige Gebiet, das Seitenbereiche enthält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Ruft die Typen der zu lesenden Barcodes ab.


**Returns:**
java.util.List<java.lang.String> - Die schreibgeschützte Sammlung, die die zu lesenden Barcode-Typen enthält; leere Sammlung, wenn nicht gesetzt ist.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Setzt den Wert, der angibt, ob falsche Barcodes erlaubt sind.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  wenn falsche Barcodes erlaubt sind. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Setzt die minimale Größe des minimalen Barcode-Elements.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dimension | java.lang.Float | Das minimale Barcode-Element;  null  für den Automatikmodus. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Setzt die Qualität eines Quellbildes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Der Bildqualitätsmodus. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Setzt die Qualität eines Quell-Barcodes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Der Barcode-Qualitätsmodus. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Setzt den rechteckigen Bereich, der Barcodes enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich;  null  zum Scannen der gesamten Seite. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Setzt die Typen der zu lesenden Barcodes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Die Barcode-Typen;  null  oder leer für alle Typen. |
|

