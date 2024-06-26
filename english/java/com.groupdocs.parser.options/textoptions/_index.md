---
title: TextOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for text extraction.
type: docs
weight: 37
url: /java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Provides the options which are used for text extraction.

An instance of [TextOptions](../../com.groupdocs.parser.options/textoptions) class is used as parameter in [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser\#getText-TextOptions-) and [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser\#getText-int--TextOptions-) methods. See the usage examples there.

It's used to specify the raw mode of text extraction. A text in this mode is extracted in a non-accurate way but faster than in the standard mode. If the raw mode doesn't support the document format, then this parameter is ignored and the standard mode is used.

**Learn more:**

 *  [Extract text in Raw Mode][]
 *  [Extract text in Accurate Mode][]


[Extract text in Raw Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode
[Extract text in Accurate Mode]: https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode
## Constructors

| Constructor | Description |
| --- | --- |
| [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Initializes a new instance of the [TextOptions](../../com.groupdocs.parser.options/textoptions) class. |
| [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Initializes a new instance of the [TextOptions](../../com.groupdocs.parser.options/textoptions) class with the OCR usage option. |
| [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Initializes a new instance of the [TextOptions](../../com.groupdocs.parser.options/textoptions) class with the ability to set OCR options. |
## Methods

| Method | Description |
| --- | --- |
| [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Gets the value that indicates whether the raw mode is used. |
| [isUseOcr()](#isUseOcr--) | Gets the value that indicates whether the OCR Connector is used to extract a text. |
| [getOcrOptions()](#getOcrOptions--) | Gets the additional options for OCR functionality. |
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Initializes a new instance of the [TextOptions](../../com.groupdocs.parser.options/textoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| useRawModeIfPossible | boolean | The value that indicates whether the raw mode is used. |

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Initializes a new instance of the [TextOptions](../../com.groupdocs.parser.options/textoptions) class with the OCR usage option.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| useRawModeIfPossible | boolean | The value that indicates whether the raw mode is used. |
| useOcr | boolean | The value that indicates whether the OCR functionality is used to extract a text. |

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Initializes a new instance of the [TextOptions](../../com.groupdocs.parser.options/textoptions) class with the ability to set OCR options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| useRawModeIfPossible | boolean | The value that indicates whether the raw mode is used. |
| useOcr | boolean | The value that indicates whether the OCR functionality is used to extract a text. |
| ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | The additional options for OCR functionality. |

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Gets the value that indicates whether the raw mode is used.

**Returns:**
boolean -  true  if the raw mode is used; otherwise,  false .
### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Gets the value that indicates whether the OCR Connector is used to extract a text.

**Returns:**
boolean -  true  if the OCR functionality is used; otherwise,  false .
### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Gets the additional options for OCR functionality.

**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.
