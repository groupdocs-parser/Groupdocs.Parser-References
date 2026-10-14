---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller mallens streckkodsfält."
type: docs
weight: 11
url: /sv/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Tillhandahåller mallens streckkodsfält.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) med namnet i STORA BOKSTÄVER. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) med namnet i STORA BOKSTÄVER. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som innehåller mallens streckkodsfält. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller mallens streckkodsfält. |
|
|  | namn | java.lang.String | Streckkodsfältets namn. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) med namnet i STORA BOKSTÄVER.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller mallens streckkodsfält. |
|
|  | namn | java.lang.String | Streckkodsfältets namn. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) med namnet i STORA BOKSTÄVER.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller mallens streckkodsfält. |
|
|  | namn | java.lang.String | Streckkodsfältets namn. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller mallens streckkodsfält. |
|
|  | namn | java.lang.String | Streckkodsfältets namn. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller mallens streckkodsfält. |
|
|  | namn | java.lang.String | Streckkodsfältets namn. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som innehåller mallens streckkodsfält.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Skapar en kopia av det aktuella objektet med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
