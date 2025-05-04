---
title: OcrConnectorBase
second_title: GroupDocs.Parser for Java API Reference
description: Provides the OCR functionality.
type: docs
weight: 25
url: /java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Provides the OCR functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [OcrConnectorBase()](#OcrConnectorBase--) | Initializes a new instance of the [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class. |
## Methods

| Method | Description |
| --- | --- |
| [isTextSupported()](#isTextSupported--) | Gets the value that indicates whether the text extraction is supported. |
| [isTextAreasSupported()](#isTextAreasSupported--) | Gets the value that indicates whether the text areas extraction is supported. |
| [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Recognize a text from  imageStream  stream. |
| [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Recognize text areas from  imageStream  stream. |
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Initializes a new instance of the [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class.

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
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The image representation of the document page. |
| options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | The OCR options. |

**Returns:**
java.lang.String - A string that represents a recognized text;  null  if text recognizing isn't supported.
### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Recognize text areas from  imageStream  stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The image representation of the document page. |
| pageSize | [Size](../../com.groupdocs.parser.data/size) | The size of the document page. |
| options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | The OCR options. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - A collection of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objects;  null  if text areas recognizing isn't supported.
