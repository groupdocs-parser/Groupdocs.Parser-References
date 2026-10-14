---
title: "TextOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för textutvinning."
type: docs
weight: 37
url: /sv/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Tillhandahåller de alternativ som används för textutvinning.

En instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) används som parameter i [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
och [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) metoder. Se användningsexemplen där.

Den används för att ange råläget för textutvinning. En text i detta läge extraheras på ett oprecist
men snabbare än i standardläget. Om råläget inte stöder dokumentformatet,
ignoreras då denna parameter och standardläget används.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med OCR-användningsalternativet. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med möjlighet att ställa in OCR-alternativ. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Hämtar värdet som indikerar om råläget används. |
|
|  | [isUseOcr()](#isUseOcr--) | Hämtar värdet som indikerar om OCR‑anslutningen används för att extrahera text. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Hämtar de extra alternativen för OCR-funktionalitet. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Hämtar värdet som indikerar om annotationer inkluderas i den extraherade texten. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Ställer in värdet som indikerar om annotationer inkluderas i den extraherade texten. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Värdet som indikerar om råläget används. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med OCR-användningsalternativet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Värdet som indikerar om råläget används. |
|
|  | useOcr | boolean | Värdet som indikerar om OCR-funktionaliteten används för att extrahera text. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Initierar en ny instans av klassen [TextOptions](../../com.groupdocs.parser.options/textoptions) med möjlighet att ställa in OCR-alternativ.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Värdet som indikerar om råläget används. |
|
|  | useOcr | boolean | Värdet som indikerar om OCR-funktionaliteten används för att extrahera text. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | De extra alternativen för OCR-funktionalitet. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Hämtar värdet som indikerar om råläget används.


**Returns:**
boolean -  true  om råläget används; annars  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Hämtar värdet som indikerar om annotationer inkluderas i den extraherade texten. Standardvärdet är  false .


**Returns:**
boolean -  true  om annotationer inkluderas; annars  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Ställer in värdet som indikerar om annotationer inkluderas i den extraherade texten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  för att inkludera annotationer i den extraherade texten. |
|

