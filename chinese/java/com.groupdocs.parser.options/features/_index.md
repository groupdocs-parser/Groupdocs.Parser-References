---
title: "Features"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示受支持的功能列表。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

表示受支持的特性列表。允许获取文档中哪些特性受支持或不受支持的信息。

此类的实例用作 [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) 属性。请参阅那里的使用示例。

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Features()](#Features--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | 返回指示该特性是否受支持的值。 |
|
|  | [isText()](#isText--) | 获取指示是否支持文本提取的值。 |
|
|  | [isTextPage()](#isTextPage--) | 获取指示是否支持文本页提取的值。 |
|
|  | [isFormattedText()](#isFormattedText--) | 获取指示是否支持格式化文本提取的值。 |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | 获取指示是否支持格式化文本页提取的值。 |
|
|  | [isSearch()](#isSearch--) | 获取指示是否支持文本搜索的值。 |
|
|  | [isHighlight()](#isHighlight--) | 获取指示是否支持突出显示提取的值。 |
|
|  | [isBarcodes()](#isBarcodes--) | 获取指示是否支持条形码提取的值。 |
|
|  | [isToc()](#isToc--) | 获取指示是否支持目录提取的值。 |
|
|  | [isMetadata()](#isMetadata--) | 获取指示是否支持元数据提取的值。 |
|
|  | [isContainer()](#isContainer--) | 获取指示是否支持容器提取的值。 |
|
|  | [isTextAreas()](#isTextAreas--) | 获取指示是否支持文本区域提取的值。 |
|
|  | [isStructure()](#isStructure--) | 获取指示是否支持文本结构提取的值。 |
|
|  | [isImages()](#isImages--) | 获取指示是否支持图像提取的值。 |
|
|  | [isHyperlinks()](#isHyperlinks--) | 获取指示是否支持超链接提取的值。 |
|
|  | [isTables()](#isTables--) | 获取指示是否支持表格提取的值。 |
|
|  | [isAnnotations()](#isAnnotations--) | 获取指示是否支持注释提取的值。 |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | 获取指示是否支持基于模板的解析的值。 |
|
|  | [isParseForm()](#isParseForm--) | 获取指示是否支持表单解析的值。 |
|
|  | [isPreview()](#isPreview--) | 获取指示是否支持预览生成的值。 |
|
|  | [isPagePreview()](#isPagePreview--) | 获取指示是否支持页面预览生成的值。 |
|
|  | [isOcr()](#isOcr--) | 获取指示是否支持 OCR 功能的值。 |
|
|  | [isWorksheet()](#isWorksheet--) | 获取指示是否支持工作表提取的值。 |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


返回指示该特性是否受支持的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | featureName | java.lang.String | 该特性名称。 |
|

**Returns:**
boolean -  true  如果支持该特性；否则，  false 。

### isText() {#isText--}
```
public boolean isText()
```


获取指示是否支持文本提取的值。


**Returns:**
boolean -  true  如果支持文本提取；否则，  false 。

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


获取指示是否支持文本页提取的值。


**Returns:**
boolean -  true  如果支持文本页面提取；否则，  false 。

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


获取指示是否支持格式化文本提取的值。


**Returns:**
boolean -  true  如果支持格式化文本提取；否则，  false 。

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


获取指示是否支持格式化文本页提取的值。


**Returns:**
boolean -  true  如果支持格式化文本页面；否则，  false 。

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


获取指示是否支持文本搜索的值。


**Returns:**
boolean -  true  如果支持文本搜索; 否则,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


获取指示是否支持突出显示提取的值。


**Returns:**
boolean -  true  如果支持高亮提取; 否则,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


获取指示是否支持条形码提取的值。


**Returns:**
boolean -  true  如果支持条形码提取; 否则,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


获取指示是否支持目录提取的值。


**Returns:**
boolean -  true  如果支持目录提取; 否则,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


获取指示是否支持元数据提取的值。


**Returns:**
boolean -  true  如果支持元数据提取; 否则,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


获取指示是否支持容器提取的值。


**Returns:**
boolean -  true  如果支持容器提取; 否则,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


获取指示是否支持文本区域提取的值。


**Returns:**
boolean -  true  如果支持文本区域提取; 否则,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


获取指示是否支持文本结构提取的值。


**Returns:**
boolean -  true  如果支持文本结构提取; 否则,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


获取指示是否支持图像提取的值。


**Returns:**
boolean -  true  如果支持图像提取; 否则,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


获取指示是否支持超链接提取的值。


**Returns:**
boolean -  true  如果支持超链接提取; 否则,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


获取指示是否支持表格提取的值。


**Returns:**
boolean -  true  如果支持表格提取; 否则,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


获取指示是否支持注释提取的值。


**Returns:**
boolean -  true  如果支持注释提取; 否则,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


获取指示是否支持基于模板的解析的值。


**Returns:**
boolean -  true  如果支持基于模板的解析; 否则,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


获取指示是否支持表单解析的值。


**Returns:**
boolean -  true  如果支持表单解析; 否则,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


获取指示是否支持预览生成的值。


**Returns:**
boolean -  true  如果支持预览生成; 否则,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


获取指示是否支持页面预览生成的值。


**Returns:**
boolean -  true  如果支持页面预览生成; 否则,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


获取指示是否支持 OCR 功能的值。


**Returns:**
boolean -  true  如果支持 OCR 功能; 否则,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


获取指示是否支持工作表提取的值。


**Returns:**
boolean -  true  如果支持工作表提取; 否则,  false .

