---
title: OcrConnectorBase
second_title: GroupDocs.Parser for Java API Reference
description: Provides the OCR functionality.
type: docs
weight: 24
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
| [recognizeText(InputStream imageStream, int pageIndex, OcrOptions options)](#recognizeText-java.io.InputStream-int-com.groupdocs.parser.options.OcrOptions-) | Recognize a text from  imageStream  stream. |
| [recognizeTextAreas(InputStream imageStream, int pageIndex, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-int-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Recognize text areas from  imageStream  stream. |
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Initializes a new instance of the [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class.

### recognizeText(InputStream imageStream, int pageIndex, OcrOptions options) {#recognizeText-java.io.InputStream-int-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, int pageIndex, OcrOptions options)
```


Recognize a text from  imageStream  stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The image representation of the document page. |
| pageIndex | int | The page index of the document. |
| options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | The OCR options. |

**Returns:**
java.lang.String - A string that represents a recognized text;  null  if text recognizing isn't supported.
### recognizeTextAreas(InputStream imageStream, int pageIndex, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-int-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, int pageIndex, Size pageSize, OcrOptions options)
```


Recognize text areas from  imageStream  stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The image representation of the document page. |
| pageIndex | int | The page index of the document. |
| pageSize | [Size](../../com.groupdocs.parser.data/size) | The size of the document page. |
| options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | The OCR options. |

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - A collection of [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) objects;  null  if text areas recognizing isn't supported.
