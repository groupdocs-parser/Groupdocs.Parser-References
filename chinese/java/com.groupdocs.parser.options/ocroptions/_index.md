---
title: "OcrOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于 OCR Connector 的选项。"
type: docs
weight: 27
url: /zh/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

提供用于 OCR Connector 的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | 使用默认值初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。 |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | 使用矩形区域初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。 |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | 使用页面预览选项初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。 |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | 使用 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 对象初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。 |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | 使用矩形区域和 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 对象初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。 |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | 初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取约束用于文本识别的页面区域的矩形区域。 |
|
|  | [getHandler()](#getHandler--) | 获取用于捕获 OCR 事件的事件处理程序。 |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | 获取指示是否使用拼写检查器的值。 |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | 获取用于渲染提供给 OCR 引擎的页面的页面预览选项。 |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | 设置用于渲染提供给 OCR 引擎的页面的页面预览选项。 |
|
|  | [getLanguage()](#getLanguage--) | 获取用于光学字符识别的语言。 |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | 设置用于光学字符识别的语言。 |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | 设置限制用于文本识别的页面区域的矩形区域。 |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | 设置用于捕获 OCR 事件的事件处理程序。 |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | 设置指示是否使用拼写检查器的值。 |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


使用默认值初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


使用矩形区域初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 限制用于文本识别的页面区域的矩形区域。 |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


使用页面预览选项初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | 用于渲染提供给 OCR 引擎的页面预览的选项。 |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


使用 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 对象初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | 用于捕获 OCR 事件的 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 实例。 |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


使用矩形区域和 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 对象初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 限制用于文本识别的页面区域的矩形区域。 |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | 用于捕获 OCR 事件的 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 实例。 |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


初始化 [OcrOptions](../../com.groupdocs.parser.options/ocroptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 限制用于文本识别的页面区域的矩形区域。 |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | 用于捕获 OCR 事件的 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 实例。 |
|
|  | useSpellCheker | boolean | 指示是否使用拼写检查器的值。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


获取约束用于文本识别的页面区域的矩形区域。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


获取用于捕获 OCR 事件的事件处理程序。


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


获取指示是否使用拼写检查器的值。


**Returns:**
boolean -  true  如果使用拼写检查器；否则为  false 。

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


获取用于渲染提供给 OCR 引擎的页面的页面预览选项。


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


设置用于渲染提供给 OCR 引擎的页面的页面预览选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | 页面预览选项。 |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


获取用于光学字符识别的语言。


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


设置用于光学字符识别的语言。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | [Language](../../com.groupdocs.parser.options/language) 枚举值。 |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


设置限制用于文本识别的页面区域的矩形区域。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 矩形，或  null  用于扫描整页。 |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


设置用于捕获 OCR 事件的事件处理程序。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | 事件处理程序。 |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


设置指示是否使用拼写检查器的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  启用拼写检查。 |
|

