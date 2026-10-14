---
title: "TextOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Textextraktion verwendet werden."
type: docs
weight: 37
url: /de/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Stellt die Optionen bereit, die für die Textextraktion verwendet werden.

Eine Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) wird als Parameter in [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-) verwendet.
und die Methoden [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) . Siehe dort die Anwendungsbeispiele.

Sie wird verwendet, um den Rohmodus der Textextraktion anzugeben. Ein Text in diesem Modus wird nicht genau
ausgegeben, aber schneller als im Standardmodus. Wenn der Rohmodus das Dokumentformat nicht unterstützt,
wird dieser Parameter ignoriert und der Standardmodus verwendet.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der OCR-Nutzungsoption. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der Möglichkeit, OCR-Optionen festzulegen. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Gibt den Wert zurück, der angibt, ob der Rohmodus verwendet wird. |
|
|  | [isUseOcr()](#isUseOcr--) | Gibt den Wert zurück, der angibt, ob der OCR-Connector zum Extrahieren eines Textes verwendet wird. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Gibt die zusätzlichen Optionen für die OCR-Funktionalität zurück. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Gibt den Wert zurück, der angibt, ob Anmerkungen im extrahierten Text enthalten sind. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Setzt den Wert, der angibt, ob Anmerkungen im extrahierten Text enthalten sind. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Der Wert, der angibt, ob der Rohmodus verwendet wird. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der OCR-Nutzungsoption.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Der Wert, der angibt, ob der Rohmodus verwendet wird. |
|
|  | useOcr | boolean | Der Wert, der angibt, ob die OCR-Funktionalität zum Extrahieren eines Textes verwendet wird. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Initialisiert eine neue Instanz der Klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) mit der Möglichkeit, OCR-Optionen festzulegen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Der Wert, der angibt, ob der Rohmodus verwendet wird. |
|
|  | useOcr | boolean | Der Wert, der angibt, ob die OCR-Funktionalität zum Extrahieren eines Textes verwendet wird. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Die zusätzlichen Optionen für die OCR-Funktionalität. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Gibt den Wert zurück, der angibt, ob der Rohmodus verwendet wird.


**Returns:**
boolean -  true  wenn der Rohmodus verwendet wird; andernfalls  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Gibt den Wert zurück, der angibt, ob Anmerkungen im extrahierten Text enthalten sind. Der Standardwert ist  false .


**Returns:**
boolean -  true  wenn Anmerkungen enthalten sind; andernfalls  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Setzt den Wert, der angibt, ob Anmerkungen im extrahierten Text enthalten sind.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  um Anmerkungen im extrahierten Text einzuschließen. |
|

