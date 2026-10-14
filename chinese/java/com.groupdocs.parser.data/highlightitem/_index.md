---
title: "HighlightItem"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文本的一部分高亮，通常用于在搜索功能中解释找到的文本的上下文。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

表示高亮，即通常用于在搜索功能中解释找到的文本上下文的文本片段。

一个 [HighlightItem](../../com.groupdocs.parser.data/highlightitem) 类的实例用作 [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) 方法的返回值，
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | 初始化一个新的 [HighlightItem](../../com.groupdocs.parser.data/highlightitem) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPosition()](#getPosition--) | 获取文档文本中的位置。 |
|
|  | [getText()](#getText--) | 获取高亮的文本。 |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


初始化一个新的 [HighlightItem](../../com.groupdocs.parser.data/highlightitem) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 位置 | int | 文档文本中的位置。 |
|
|  | 文本 | java.lang.String | 高亮的文本。 |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


获取文档文本中的位置。


**Returns:**
int - 高亮起始位置的零基索引。

### getText() {#getText--}
```
public String getText()
```


获取高亮的文本。


**Returns:**
java.lang.String - 表示高亮文本的字符串值。

