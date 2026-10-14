---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor het extraheren van paginatekstgebieden."
type: docs
weight: 32
url: /nl/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Biedt de opties die worden gebruikt voor het extraheren van paginatekstgebieden.

Een instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) wordt gebruikt als parameter in [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
en [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) methoden. Zie de gebruiksvoorbeelden daar.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met standaardwaarden. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de OCR-gebruikoptie. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de mogelijkheid om OCR-opties in te stellen. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de reguliere expressie. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de reguliere expressie en rechthoekig gebied. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de reguliere expressie, rechthoekig gebied en de grootte van de genegeerde rand. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de grootte van de genegeerde rand. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getExpression()](#getExpression--) | Haalt de reguliere expressie op. |
|
|  | [isMatchCase()](#isMatchCase--) | Haalt de waarde op die aangeeft of hoofdlettergebruik van tekst niet wordt genegeerd. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Haalt de waarde op die aangeeft of segmenten worden samengevoegd. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Haalt de waarde op die aangeeft of tekstopmaak wordt genegeerd. |
|
|  | [isUseOcr()](#isUseOcr--) | Haalt de waarde op die aangeeft of de OCR-connector wordt gebruikt om een tekst te extraheren. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Haalt de aanvullende opties voor OCR-functionaliteit op. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met standaardwaarden.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de OCR-gebruikoptie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | useOcr | boolean | De waarde die aangeeft of de OCR-functionaliteit wordt gebruikt om een tekst te extraheren. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de mogelijkheid om OCR-opties in te stellen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | useOcr | boolean | De waarde die aangeeft of de OCR-functionaliteit wordt gebruikt om een tekst te extraheren. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | De aanvullende opties voor OCR-functionaliteit. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de reguliere expressie. Andere opties worden standaard ingesteld (zie opmerkingen voor details).

De volgende eigenschappen hebben standaardwaarden:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de reguliere expressie en rechthoekig gebied. Andere opties worden standaard ingesteld (zie opmerkingen voor details).

De volgende eigenschappen hebben standaardwaarden:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat pagina‑gebieden bevat. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de reguliere expressie, rechthoekig gebied en de grootte van de genegeerde rand. Andere opties worden standaard ingesteld (zie opmerkingen voor details).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat pagina‑gebieden bevat. |
|
|  | rectangleTolerance | double | De grootte van de rand die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Deze wordt gemeten als een fractie van de hoogte van een tekstelement. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | uniteSegments | boolean | De waarde die aangeeft of segmenten zijn verenigd. |
|
|  | ignoreFormatting | boolean | De waarde die aangeeft of tekstopmaak wordt genegeerd. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat pagina‑gebieden bevat. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Initialiseert een nieuwe instantie van de klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) met de grootte van de genegeerde rand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | expression | java.lang.String | De reguliere expressie. |
|
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | uniteSegments | boolean | De waarde die aangeeft of segmenten zijn verenigd. |
|
|  | ignoreFormatting | boolean | De waarde die aangeeft of tekstopmaak wordt genegeerd. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat pagina‑gebieden bevat. |
|
|  | rectangleTolerance | double | De grootte van de rand die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Deze wordt gemeten als een fractie van de hoogte van een tekstelement. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Haalt de reguliere expressie op.


**Returns:**
java.lang.String - Een string die de reguliere expressie vertegenwoordigt.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Haalt de waarde op die aangeeft of hoofdlettergebruik van tekst niet wordt genegeerd.


**Returns:**
boolean -  true  als een tekstcase niet wordt genegeerd; anders,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Haalt de waarde op die aangeeft of segmenten worden samengevoegd.


**Returns:**
boolean - {code true} als segmenten zijn verenigd; anders, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Haalt de waarde op die aangeeft of tekstopmaak wordt genegeerd.


**Returns:**
boolean -  true  als tekstopmaak wordt genegeerd; anders,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Haalt de waarde op die aangeeft of de OCR-connector wordt gebruikt om een tekst te extraheren.


**Returns:**
boolean -  true  als de OCR-functionaliteit wordt gebruikt; anders,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Haalt de aanvullende opties voor OCR-functionaliteit op.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

