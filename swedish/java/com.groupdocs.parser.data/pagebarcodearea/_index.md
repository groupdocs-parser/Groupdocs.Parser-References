---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett sidområde för streckkod som används för att representera ett streckkodsvärde i funktionaliteten för parsning med mall."
type: docs
weight: 18
url: /sv/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Representerar ett sidområde för streckkod som används för att representera ett streckkodsvärde i funktionaliteten för parsning med mall.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getValue()](#getValue--) | Hämtar streckkodsvärdet. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Hämtar namnet på streckkodstypen. |
|
|  | [getConfidence()](#getConfidence--) | Hämtar förtroendenivån för den analyserade streckkoden. |
|
|  | [getAngle()](#getAngle--) | Hämtar vinkeln på streckkoden. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Värdet på streckkoden. |
|
|  | codeTypeName | java.lang.String | Typnamnet för streckkoden. |
|
|  | confidence | int | Nivån av förtroende för den parsade streckkoden. |
|
|  | vinkel | double | Vinkeln på streckkoden. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller streckkodsområdet. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller streckkodsområdet. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Hämtar streckkodsvärdet.


**Returns:**
java.lang.String - Ett strängvärde som representerar ett värde för streckkodens sidområde.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Hämtar namnet på streckkodstypen.


**Returns:**
java.lang.String - Ett strängvärde som representerar ett typnamn för streckkoden.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Hämtar förtroendenivån för den analyserade streckkoden.


**Returns:**
int - Ett heltalsvärde som representerar förtroendet för den parsade streckkoden (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Hämtar vinkeln på streckkoden.


**Returns:**
double - Ett flyttalsvärde som representerar vinkeln på streckkoden (0-360).

