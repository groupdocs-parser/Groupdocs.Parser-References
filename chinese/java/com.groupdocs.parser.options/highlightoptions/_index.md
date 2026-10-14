---
title: "HighlightOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于在搜索场景中提取位于找到的文本周围的文本块的选项。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

提供用于提取高亮（在搜索场景中围绕找到的文本的文本块）的选项。

在 [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) 方法中，使用 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的实例作为参数。
请参阅那里的使用示例。

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | 初始化一个未设置限制的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。 |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | 初始化一个用于提取固定长度高亮的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。 |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | 初始化一个用于提取行限制高亮的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。 |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | 初始化一个用于提取具有固定字数的高亮的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。 |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | 初始化 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | 获取最大文本长度。 |
|
|  | [getWordCount()](#getWordCount--) | 获取最大字数。 |
|
|  | [isLineLimited()](#isLineLimited--) | 获取指示高亮提取是否受文本行的起始（或结束）限制的值。 |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | 设置最大文本长度。 |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | 设置最大字数。 |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | 设置指示高亮提取是否受文本行的起始（或结束）限制的值。 |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


初始化一个未设置限制的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。在传递给解析器之前，请至少设置以下之一：#setMaxLength(Integer).setMaxLength(Integer)、#setWordCount(Integer).setWordCount(Integer)、#setLineLimited(boolean).setLineLimited(boolean)。


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


初始化一个用于提取固定长度高亮的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | maxLength | int | 最大文本长度。 |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


初始化一个用于提取行限制高亮的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 最大文本长度。 |
|
|  | isLineLimited | boolean | 指示突出显示提取是否受文本行的起始（或结束）限制的值。 |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


初始化一个用于提取具有固定字数的高亮的 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 最大文本长度。 |
|
|  | wordCount | int | 最大单词数。 |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


初始化 [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 最大文本长度。 |
|
|  | wordCount | java.lang.Integer | 最大单词数。 |
|
|  | isLineLimited | boolean | 指示突出显示提取是否受文本行的起始（或结束）限制的值。 |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


获取最大文本长度。


**Returns:**
java.lang.Integer - 表示最大文本长度的正整数值；  null  表示文本长度未受限制。

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


获取最大字数。


**Returns:**
java.lang.Integer - 表示最大单词数的正整数值；  null  表示单词数未受限制。

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


获取指示高亮提取是否受文本行的起始（或结束）限制的值。


**Returns:**
boolean -  true  如果突出显示提取受文本行的起始（或结束）限制；否则为  false 。

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


设置最大文本长度。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | 非负整数；  null  表示移除长度限制。 |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


设置最大字数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | 非负整数；  null  表示移除单词计数限制。 |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


设置指示高亮提取是否受文本行的起始（或结束）限制的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lineLimited | boolean | true  表示按行边界限制。 |
|

