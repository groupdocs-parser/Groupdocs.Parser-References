---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een paginabarcoderegio voor die wordt gebruikt om een barcodelabel te representeren in de functionaliteit voor parsing op basis van sjablonen."
type: docs
weight: 18
url: /nl/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Stelt een paginabarcoderegio voor die wordt gebruikt om een barcodelabel te representeren in de functionaliteit voor parsing op basis van sjablonen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getValue()](#getValue--) | Haalt de barcodewaarde op. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Haalt de naam van het barcode-type op. |
|
|  | [getConfidence()](#getConfidence--) | Haalt het vertrouwensniveau van de geparseerde barcode op. |
|
|  | [getAngle()](#getAngle--) | Haalt de hoek van de barcode op. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De waarde van de barcode. |
|
|  | codeTypeName | java.lang.String | De typenaam van de barcode. |
|
|  | confidence | int | Het vertrouwensniveau van de geparseerde barcode. |
|
|  | angle | double | De hoek van de barcode. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die het barcodegebied bevat. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het barcodegebied bevat. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Haalt de barcodewaarde op.


**Returns:**
java.lang.String - Een tekenreekswaarde die een waarde van het barcode-pagina-gebied vertegenwoordigt.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Haalt de naam van het barcode-type op.


**Returns:**
java.lang.String - Een tekenreekswaarde die een typenaam van de barcode vertegenwoordigt.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Haalt het vertrouwensniveau van de geparseerde barcode op.


**Returns:**
int - Een geheel getal dat de betrouwbaarheid van de geparseerde barcode weergeeft (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Haalt de hoek van de barcode op.


**Returns:**
double - Een geheel getal dat de hoek van de barcode weergeeft (0-360).

