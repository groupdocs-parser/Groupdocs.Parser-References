---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于格式化文本提取的选项。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

提供用于格式化文本提取的选项。

在 [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-) 方法中使用 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 类的实例作为参数。
以及 [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) 方法。请参阅那里的使用示例。

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | 初始化一个未设置模式的 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 类的新实例。 |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | 初始化 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getMode()](#getMode--) | 获取格式化文本提取模式。 |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | 设置格式化文本提取模式。 |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


初始化一个未设置模式的 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 类的新实例。


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


初始化 [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | 格式化文本提取的模式。 |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


获取格式化文本提取模式。


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


设置格式化文本提取模式。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) 枚举，包含格式化文本提取模式。 |
|

