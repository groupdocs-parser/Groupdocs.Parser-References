---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller OCR-funktionaliteten."
type: docs
weight: 25
url: /sv/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Tillhandahåller OCR-funktionaliteten.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Initierar en ny instans av klassen [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) klass. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Hämtar värdet som indikerar om textutdrag stöds. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Hämtar värdet som indikerar om extrahering av textområden stöds. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Känn igen en text från  imageStream  ström. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Känn igen textområden från  imageStream  ström. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Initierar en ny instans av klassen [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) klass.


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Hämtar värdet som indikerar om textutdrag stöds.


**Returns:**
boolean -  true  om textutdrag stöds; annars,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Hämtar värdet som indikerar om extrahering av textområden stöds.


**Returns:**
boolean -  true  om extrahering av textområden stöds; annars,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Känn igen en text från  imageStream  ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Bildrepresentationen av dokumentsidan. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR-alternativen. |
|

**Returns:**
java.lang.String - En sträng som representerar en erkänd text;  null  om textigenkänning inte stöds.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Känn igen textområden från  imageStream  ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Bildrepresentationen av dokumentsidan. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | Storleken på dokumentsidan. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR-alternativen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - En samling av [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objekt;  null  om igenkänning av textområden inte stöds.

