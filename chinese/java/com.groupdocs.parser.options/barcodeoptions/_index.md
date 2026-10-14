---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于条形码提取的选项。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

提供用于条形码提取的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | 使用默认值初始化 BarcodeOptions 类的新实例。 |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | 使用矩形区域初始化 BarcodeOptions 类的新实例。 |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | 使用质量设置和代码类型初始化 BarcodeOptions 类的新实例。 |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | 初始化 BarcodeOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | 获取指示是否允许不正确条形码的值。 |
|
|  | [getDimension()](#getDimension--) | 获取条形码最小元素的最小尺寸。 |
|
|  | [getImageQuality()](#getImageQuality--) | 获取源图像的质量。 |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | 获取源条形码的质量。 |
|
|  | [getRectangle()](#getRectangle--) | 获取包含页面区域的矩形区域。 |
|
|  | [getCodeTypes()](#getCodeTypes--) | 获取要读取的条形码类型。 |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | 设置指示是否允许不正确条形码的值。 |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | 设置条形码最小元素的最小尺寸。 |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | 设置源图像的质量。 |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | 设置源条形码的质量。 |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | 设置包含条形码的矩形区域。 |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | 设置要读取的条形码类型。 |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


使用默认值初始化 BarcodeOptions 类的新实例。


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


使用矩形区域初始化 BarcodeOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含条形码的矩形区域。 |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


使用质量设置和代码类型初始化 BarcodeOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 源图像的质量。 |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 源条形码的质量。 |
|
|  | codeTypes | java.lang.String[] | 要读取的条形码类型。 |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


初始化 BarcodeOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含条形码的矩形区域。 |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 源图像的质量。 |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 源条形码的质量。 |
|
|  | dimension | java.lang.Float | 条形码最小元素的最小尺寸。 |
|
|  | allowIncorrectBarcodes | boolean | 指示是否允许不正确条形码的值。 |
|
|  | codeTypes | java.lang.String[] | 要读取的条形码类型。 |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


获取指示是否允许不正确条形码的值。


**Returns:**
boolean -  true  如果允许不正确的条形码；否则， false 。

### getDimension() {#getDimension--}
```
public Float getDimension()
```


获取条形码最小元素的最小尺寸。


**Returns:**
java.lang.Float - 表示条形码最小元素的浮点值；如果使用自动模式则为 null。

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


获取源图像的质量。


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


获取源条形码的质量。


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取包含页面区域的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


获取要读取的条形码类型。


**Returns:**
java.util.List<java.lang.String> - 包含要读取的条形码类型的只读集合；如果未设置则为空集合。

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


设置指示是否允许不正确条形码的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | 如果允许不正确的条形码，则为 true。 |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


设置条形码最小元素的最小尺寸。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | dimension | java.lang.Float | 条形码最小元素；自动模式时为 null。 |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


设置源图像的质量。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 图像质量模式。 |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


设置源条形码的质量。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | 条形码质量模式。 |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


设置包含条形码的矩形区域。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 矩形区域；若为 null 则扫描整页。 |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


设置要读取的条形码类型。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | 条形码类型；null 或空表示所有类型。 |
|

