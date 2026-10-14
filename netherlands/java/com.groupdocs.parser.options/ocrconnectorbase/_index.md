---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de OCR-functionaliteit."
type: docs
weight: 25
url: /nl/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Biedt de OCR-functionaliteit.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Initialiseert een nieuw exemplaar van de [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Haalt de waarde op die aangeeft of de tekstextractie wordt ondersteund. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Haalt de waarde op die aangeeft of de extractie van tekstgebieden wordt ondersteund. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Herken een tekst uit  imageStream  stream. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Herken tekstgebieden uit  imageStream  stream. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Initialiseert een nieuw exemplaar van de [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) klasse.


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Haalt de waarde op die aangeeft of de tekstextractie wordt ondersteund.


**Returns:**
boolean -  true  als de tekstextractie wordt ondersteund; anders,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Haalt de waarde op die aangeeft of de extractie van tekstgebieden wordt ondersteund.


**Returns:**
boolean -  true  als de extractie van tekstgebieden wordt ondersteund; anders,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Herken een tekst uit  imageStream  stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | De afbeeldingrepresentatie van de documentpagina. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | De OCR‑opties. |
|

**Returns:**
java.lang.String - Een string die een herkende tekst vertegenwoordigt;  null  als tekstherkenning niet wordt ondersteund.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Herken tekstgebieden uit  imageStream  stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | De afbeeldingrepresentatie van de documentpagina. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | De grootte van de documentpagina. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | De OCR‑opties. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Een verzameling van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objecten;  null  als herkenning van tekstgebieden niet wordt ondersteund.

