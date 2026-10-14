---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die OCR-Funktionalität bereit."
type: docs
weight: 25
url: /de/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Stellt die OCR-Funktionalität bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Initialisiert eine neue Instanz der Klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Gets the value that indicates whether the text extraction is supported. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Gets the value that indicates whether the text areas extraction is supported. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Recognize a text from  imageStream  stream. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Recognize text areas from  imageStream  stream. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Initialisiert eine neue Instanz der Klasse [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Gets the value that indicates whether the text extraction is supported.


**Returns:**
boolean -  true  if the text extraction is supported; otherwise,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Gets the value that indicates whether the text areas extraction is supported.


**Returns:**
boolean -  true  if the text extraction areas is supported; otherwise,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Recognize a text from  imageStream  stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Die Bilddarstellung der Dokumentseite. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Die OCR-Optionen. |
|

**Returns:**
java.lang.String - Ein String, der einen erkannten Text darstellt;  null  wenn die Texterkennung nicht unterstützt wird.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Recognize text areas from  imageStream  stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Die Bilddarstellung der Dokumentseite. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | Die Größe der Dokumentseite. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Die OCR-Optionen. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Eine Sammlung von [PageTextArea](../../com.groupdocs.parser.data/pagetextarea)-Objekten;  null  wenn die Erkennung von Textbereichen nicht unterstützt wird.

