---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于页面文本区域提取的选项。"
type: docs
weight: 32
url: /zh/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

提供用于页面文本区域提取的选项。

在 [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-) 中，使用 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的实例作为参数。
以及 [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) 方法。请参阅那里的使用示例。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | 使用默认值初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。 |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | 使用 OCR 使用选项初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例。 |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | 初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例，以便设置 OCR 选项。 |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | 使用正则表达式初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。 |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | 使用正则表达式和矩形区域初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。 |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | 使用正则表达式、矩形区域以及忽略边框的大小初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。 |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | 初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。 |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | 使用忽略边框的大小初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getExpression()](#getExpression--) | 获取正则表达式。 |
|
|  | [isMatchCase()](#isMatchCase--) | 获取指示文本大小写是否未被忽略的值。 |
|
|  | [isUniteSegments()](#isUniteSegments--) | 获取指示段是否已合并的值。 |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | 获取指示文本格式是否被忽略的值。 |
|
|  | [isUseOcr()](#isUseOcr--) | 获取指示是否使用 OCR 连接器提取文本的值。 |
|
|  | [getOcrOptions()](#getOcrOptions--) | 获取 OCR 功能的附加选项。 |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


使用默认值初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


使用 OCR 使用选项初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | useOcr | boolean | 指示是否使用 OCR 功能提取文本的值。 |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例，以便设置 OCR 选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | useOcr | boolean | 指示是否使用 OCR 功能提取文本的值。 |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 功能的附加选项。 |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


使用正则表达式初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。其他选项使用默认值（详见备注）。

以下属性具有默认值：

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


使用正则表达式和矩形区域初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。其他选项使用默认值（详见备注）。

以下属性具有默认值：

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含页面区域的矩形区域。 |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


使用正则表达式、矩形区域和忽略边框的大小初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。其他选项使用默认值（详见备注）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含页面区域的矩形区域。 |
|
|  | rectangleTolerance | double | 在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。 |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | uniteSegments | boolean | 指示段是否已合并的值。 |
|
|  | ignoreFormatting | boolean | 指示文本格式是否被忽略的值。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含页面区域的矩形区域。 |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


使用忽略边框的大小初始化 [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | expression | java.lang.String | 正则表达式。 |
|
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | uniteSegments | boolean | 指示段是否已合并的值。 |
|
|  | ignoreFormatting | boolean | 指示文本格式是否被忽略的值。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含页面区域的矩形区域。 |
|
|  | rectangleTolerance | double | 在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。 |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


获取正则表达式。


**Returns:**
java.lang.String - 表示正则表达式的字符串。

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


获取指示文本大小写是否未被忽略的值。


**Returns:**
boolean -  true  如果文本大小写未被忽略；否则，  false 。

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


获取指示段是否已合并的值。


**Returns:**
boolean - {code true} 如果段已合并；否则，{code false}。

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


获取指示文本格式是否被忽略的值。


**Returns:**
boolean -  true  如果文本格式被忽略；否则，  false 。

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


获取指示是否使用 OCR 连接器提取文本的值。


**Returns:**
boolean -  true  表示使用 OCR 功能；否则为  false 。

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


获取 OCR 功能的附加选项。


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

