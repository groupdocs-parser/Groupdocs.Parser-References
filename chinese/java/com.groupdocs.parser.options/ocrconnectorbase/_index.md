---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供 OCR 功能。"
type: docs
weight: 25
url: /zh/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

提供 OCR 功能。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | 初始化 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | 获取指示是否支持文本提取的值。 |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | 获取指示是否支持文本区域提取的值。 |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | 从  imageStream  流中识别文本。 |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | 从  imageStream  流中识别文本区域。 |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


初始化 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 类的新实例。


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


获取指示是否支持文本提取的值。


**Returns:**
boolean -  true  如果支持文本提取; 否则,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


获取指示是否支持文本区域提取的值。


**Returns:**
boolean -  true  如果支持文本提取区域; 否则,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


从  imageStream  流中识别文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 文档页的图像表示。 |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 选项。 |
|

**Returns:**
java.lang.String - 表示已识别文本的字符串;  null  如果不支持文本识别。

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


从  imageStream  流中识别文本区域。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 文档页的图像表示。 |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | 文档页的大小。 |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 选项。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) 对象的集合;  null  如果不支持文本区域识别。

