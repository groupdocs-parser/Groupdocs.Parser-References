---
title: BarcodeOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for barcode extraction.
type: docs
weight: 10
url: /java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Provides the options which are used for barcode extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [BarcodeOptions()](#BarcodeOptions--) | Initializes a new instance of the BarcodeOptions class with default values. |
| [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the BarcodeOptions class with the rectangular area. |
| [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Initializes a new instance of the BarcodeOptions class with quality settings and code types. |
| [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Initializes a new instance of the BarcodeOptions class. |
## Methods

| Method | Description |
| --- | --- |
| [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Gets the value that indicates whether the incorrect barcodes are allowed. |
| [getDimension()](#getDimension--) | Gets the minimal size of the barcode minimal element. |
| [getImageQuality()](#getImageQuality--) | Gets the quality of a source image. |
| [getBarcodeQuality()](#getBarcodeQuality--) | Gets the quality of a source barcode. |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that contains page areas. |
| [getCodeTypes()](#getCodeTypes--) | Gets the types of barcodes to read. |
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Initializes a new instance of the BarcodeOptions class with default values.

### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Initializes a new instance of the BarcodeOptions class with the rectangular area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains barcodes. |

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Initializes a new instance of the BarcodeOptions class with quality settings and code types.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | The quality of a source image. |
| barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | The quality of a source barcode. |
| codeTypes | java.lang.String[] | The types of barcodes to read. |

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Initializes a new instance of the BarcodeOptions class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains barcodes. |
| imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | The quality of a source image. |
| barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | The quality of a source barcode. |
| dimension | java.lang.Float | The minimal size of the barcode minimal element. |
| allowIncorrectBarcodes | boolean | The value that indicates whether the incorrect barcodes are allowed. |
| codeTypes | java.lang.String[] | The types of barcodes to read. |

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Gets the value that indicates whether the incorrect barcodes are allowed.

**Returns:**
boolean
### getDimension() {#getDimension--}
```
public Float getDimension()
```


Gets the minimal size of the barcode minimal element.

**Returns:**
java.lang.Float
### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Gets the quality of a source image.

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Gets the quality of a source barcode.

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that contains page areas.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle)
### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Gets the types of barcodes to read.

**Returns:**
java.util.List<java.lang.String>
