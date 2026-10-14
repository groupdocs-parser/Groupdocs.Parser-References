---
title: "TextOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor tekstextractie."
type: docs
weight: 37
url: /nl/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Biedt de opties die worden gebruikt voor tekstextractie.

Een instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) wordt gebruikt als parameter in [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
en de methoden [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) . Zie de gebruiksvoorbeelden daar.

Het wordt gebruikt om de ruwe modus van tekste-extractie op te geven. Een tekst in deze modus wordt geëxtraheerd op een niet-nauwkeurige
manier, maar sneller dan in de standaardmodus. Als de ruwe modus het documentformaat niet ondersteunt,
dan wordt deze parameter genegeerd en wordt de standaardmodus gebruikt.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de OCR-gebruikoptie. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de mogelijkheid om OCR-opties in te stellen. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Haalt de waarde op die aangeeft of de ruwe modus wordt gebruikt. |
|
|  | [isUseOcr()](#isUseOcr--) | Haalt de waarde op die aangeeft of de OCR-connector wordt gebruikt om een tekst te extraheren. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Haalt de aanvullende opties voor OCR-functionaliteit op. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Haalt de waarde op die aangeeft of annotaties zijn opgenomen in de geëxtraheerde tekst. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Stelt de waarde in die aangeeft of annotaties zijn opgenomen in de geëxtraheerde tekst. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | De waarde die aangeeft of de ruwe modus wordt gebruikt. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de OCR-gebruikoptie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | De waarde die aangeeft of de ruwe modus wordt gebruikt. |
|
|  | useOcr | boolean | De waarde die aangeeft of de OCR-functionaliteit wordt gebruikt om een tekst te extraheren. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Initialiseert een nieuwe instantie van de klasse [TextOptions](../../com.groupdocs.parser.options/textoptions) met de mogelijkheid om OCR-opties in te stellen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | De waarde die aangeeft of de ruwe modus wordt gebruikt. |
|
|  | useOcr | boolean | De waarde die aangeeft of de OCR-functionaliteit wordt gebruikt om een tekst te extraheren. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | De aanvullende opties voor OCR-functionaliteit. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Haalt de waarde op die aangeeft of de ruwe modus wordt gebruikt.


**Returns:**
boolean -  true  als de ruwe modus wordt gebruikt; anders,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Haalt de waarde op die aangeeft of annotaties zijn opgenomen in de geëxtraheerde tekst. De standaardwaarde is  false .


**Returns:**
boolean -  true  als annotaties zijn opgenomen; anders,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Stelt de waarde in die aangeeft of annotaties zijn opgenomen in de geëxtraheerde tekst.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  om annotaties op te nemen in de geëxtraheerde tekst. |
|

