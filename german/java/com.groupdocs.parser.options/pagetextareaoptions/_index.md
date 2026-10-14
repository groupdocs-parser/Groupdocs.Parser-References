---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion von Textbereichen einer Seite verwendet werden."
type: docs
weight: 32
url: /de/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Stellt die Optionen bereit, die für die Extraktion von Textbereichen einer Seite verwendet werden.

Eine Instanz der Klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) wird als Parameter in [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-) verwendet.
und die Methoden [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) . Siehe die dortigen Anwendungsbeispiele.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Initialisiert eine neue Instanz der Klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) mit Standardwerten. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der OCR-Nutzungsoption. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der Möglichkeit, OCR-Optionen festzulegen. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) mit dem regulären Ausdruck. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) mit dem regulären Ausdruck und dem rechteckigen Bereich. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse mit dem regulären Ausdruck, dem rechteckigen Bereich und der Größe des zu ignorierenden Randes. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse mit der Größe des zu ignorierenden Randes. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getExpression()](#getExpression--) | Liefert den regulären Ausdruck. |
|
|  | [isMatchCase()](#isMatchCase--) | Liefert den Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Liefert den Wert, der angibt, ob Segmente vereinigt sind. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Liefert den Wert, der angibt, ob die Textformatierung ignoriert wird. |
|
|  | [isUseOcr()](#isUseOcr--) | Gibt den Wert zurück, der angibt, ob der OCR-Connector zum Extrahieren eines Textes verwendet wird. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Gibt die zusätzlichen Optionen für die OCR-Funktionalität zurück. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Initialisiert eine neue Instanz der Klasse [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) mit Standardwerten.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der OCR-Nutzungsoption.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | useOcr | boolean | Der Wert, der angibt, ob die OCR-Funktionalität zum Extrahieren eines Textes verwendet wird. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der Möglichkeit, OCR-Optionen festzulegen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | useOcr | boolean | Der Wert, der angibt, ob die OCR-Funktionalität zum Extrahieren eines Textes verwendet wird. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Die zusätzlichen Optionen für die OCR-Funktionalität. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse mit dem regulären Ausdruck. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details).

Die folgenden Eigenschaften haben Standardwerte:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse mit dem regulären Ausdruck und dem rechteckigen Bereich. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details).

Die folgenden Eigenschaften haben Standardwerte:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das rechteckige Gebiet, das Seitenbereiche enthält. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse mit dem regulären Ausdruck, dem rechteckigen Bereich und der Größe des zu ignorierenden Randes. Andere Optionen werden standardmäßig gesetzt (siehe Anmerkungen für Details).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das rechteckige Gebiet, das Seitenbereiche enthält. |
|
|  | rectangleTolerance | double | Die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | uniteSegments | boolean | Der Wert, der angibt, ob Segmente vereinigt sind. |
|
|  | ignoreFormatting | boolean | Der Wert, der angibt, ob die Textformatierung ignoriert wird. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das rechteckige Gebiet, das Seitenbereiche enthält. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Initialisiert eine neue Instanz der [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions)-Klasse mit der Größe des zu ignorierenden Randes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | expression | java.lang.String | Der reguläre Ausdruck. |
|
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | uniteSegments | boolean | Der Wert, der angibt, ob Segmente vereinigt sind. |
|
|  | ignoreFormatting | boolean | Der Wert, der angibt, ob die Textformatierung ignoriert wird. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das rechteckige Gebiet, das Seitenbereiche enthält. |
|
|  | rectangleTolerance | double | Die Größe des Randes, der beim Erfassen durch das rechteckige Gebiet ignoriert wird. Sie wird als Bruchteil der Höhe eines Textelements gemessen. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Liefert den regulären Ausdruck.


**Returns:**
java.lang.String - Eine Zeichenkette, die den regulären Ausdruck darstellt.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Liefert den Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird.


**Returns:**
boolean -  true  wenn die Groß-/Kleinschreibung nicht ignoriert wird; andernfalls  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Liefert den Wert, der angibt, ob Segmente vereinigt sind.


**Returns:**
boolean - {code true} wenn Segmente vereinigt sind; andernfalls, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Liefert den Wert, der angibt, ob die Textformatierung ignoriert wird.


**Returns:**
boolean -  true  wenn die Textformatierung ignoriert wird; andernfalls,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Gibt den Wert zurück, der angibt, ob der OCR-Connector zum Extrahieren eines Textes verwendet wird.


**Returns:**
boolean -  true  wenn die OCR-Funktionalität verwendet wird; andernfalls  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Gibt die zusätzlichen Optionen für die OCR-Funktionalität zurück.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

