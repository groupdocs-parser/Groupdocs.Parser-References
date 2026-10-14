---
title: "TextOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于文本提取的选项。"
type: docs
weight: 37
url: /zh/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

提供用于文本提取的选项。

一个 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类的实例用作 [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-) 方法的参数。
以及 [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) 方法。请参阅那里的使用示例。

它用于指定文本提取的原始模式。该模式下的文本以非精确的方式提取
但速度快于标准模式。如果原始模式不支持文档格式，
则此参数将被忽略，并使用标准模式。

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | 初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例。 |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | 使用 OCR 使用选项初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例。 |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | 初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例，以便设置 OCR 选项。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | 获取指示是否使用原始模式的值。 |
|
|  | [isUseOcr()](#isUseOcr--) | 获取指示是否使用 OCR 连接器提取文本的值。 |
|
|  | [getOcrOptions()](#getOcrOptions--) | 获取 OCR 功能的附加选项。 |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | 获取指示是否在提取的文本中包含批注的值。 |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | 设置指示是否在提取的文本中包含批注的值。 |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 指示是否使用原始模式的值。 |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


使用 OCR 使用选项初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 指示是否使用原始模式的值。 |
|
|  | useOcr | boolean | 指示是否使用 OCR 功能提取文本的值。 |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


初始化一个新的 [TextOptions](../../com.groupdocs.parser.options/textoptions) 类实例，以便设置 OCR 选项。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 指示是否使用原始模式的值。 |
|
|  | useOcr | boolean | 指示是否使用 OCR 功能提取文本的值。 |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 功能的附加选项。 |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


获取指示是否使用原始模式的值。


**Returns:**
boolean -  true  表示使用原始模式；否则为  false 。

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


获取指示是否在提取的文本中包含批注的值。默认值为  false 。


**Returns:**
boolean -  true  表示包含批注；否则为  false 。

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


设置指示是否在提取的文本中包含批注的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  表示在提取的文本中包含批注。 |
|

