---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för extrahering av sidtextområden."
type: docs
weight: 32
url: /sv/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Tillhandahåller de alternativ som används för extrahering av sidtextområden.

En instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) används som parameter i [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
och metoderna [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) . Se exempel på användning där.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med standardvärden. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med OCR-användningsalternativet. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med möjlighet att ställa in OCR-alternativ. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med det reguljära uttrycket. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med det reguljära uttrycket och rektangulärt område. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med det reguljära uttrycket, rektangulärt område och storleken på den ignorerade kanten. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med storleken på den ignorerade kanten. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getExpression()](#getExpression--) | Hämtar det reguljära uttrycket. |
|
|  | [isMatchCase()](#isMatchCase--) | Hämtar värdet som indikerar om ett textfall inte ignoreras. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Hämtar värdet som indikerar om segment är förenade. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Hämtar värdet som indikerar om textformatering ignoreras. |
|
|  | [isUseOcr()](#isUseOcr--) | Hämtar värdet som indikerar om OCR‑anslutningen används för att extrahera text. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Hämtar de extra alternativen för OCR-funktionalitet. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med standardvärden.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med OCR-användningsalternativet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | useOcr | boolean | Värdet som indikerar om OCR-funktionaliteten används för att extrahera text. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med möjlighet att ställa in OCR-alternativ.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | useOcr | boolean | Värdet som indikerar om OCR-funktionaliteten används för att extrahera text. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | De extra alternativen för OCR-funktionalitet. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med reguljärt uttryck. Övriga alternativ är förinställda (se kommentarer för detaljer).

Följande egenskaper har standardvärden:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med reguljärt uttryck och rektangulärt område. Övriga alternativ är förinställda (se kommentarer för detaljer).

Följande egenskaper har standardvärden:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller sidområden. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med reguljärt uttryck, rektangulärt område och storleken på den ignorerade kanten. Övriga alternativ är förinställda (se kommentarer för detaljer).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller sidområden. |
|
|  | rectangleTolerance | double | Storleken på kanten som ignoreras när den fångas av det rektangulära området. Den mäts som en bråkdel av en textrads höjd. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | uniteSegments | boolean | Värdet som indikerar om segmenten förenas. |
|
|  | ignoreFormatting | boolean | Värdet som indikerar om textformatering ignoreras. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller sidområden. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Initierar en ny instans av klassen [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) med storleken på den ignorerade kanten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | expression | java.lang.String | Det reguljära uttrycket. |
|
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | uniteSegments | boolean | Värdet som indikerar om segmenten förenas. |
|
|  | ignoreFormatting | boolean | Värdet som indikerar om textformatering ignoreras. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller sidområden. |
|
|  | rectangleTolerance | double | Storleken på kanten som ignoreras när den fångas av det rektangulära området. Den mäts som en bråkdel av en textrads höjd. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Hämtar det reguljära uttrycket.


**Returns:**
java.lang.String - En sträng som representerar det reguljära uttrycket.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Hämtar värdet som indikerar om ett textfall inte ignoreras.


**Returns:**
boolean -  true  om skiftläge i texten inte ignoreras; annars,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Hämtar värdet som indikerar om segment är förenade.


**Returns:**
boolean - {code true} om segmenten förenas; annars, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Hämtar värdet som indikerar om textformatering ignoreras.


**Returns:**
boolean -  true  om textformatering ignoreras; annars,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Hämtar värdet som indikerar om OCR‑anslutningen används för att extrahera text.


**Returns:**
boolean -  true  om OCR-funktionaliteten används; annars  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Hämtar de extra alternativen för OCR-funktionalitet.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

