---
title: "SearchResult"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示搜索功能中的搜索结果。"
type: docs
weight: 27
url: /zh/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

表示搜索功能中的搜索结果。

SearchResult 类的实例用作 [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-) 的返回值。
以及 [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) 方法。请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | 初始化一个新的 [SearchResult](../../com.groupdocs.parser.data/searchresult) 类实例。 |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | 初始化一个新的 [SearchResult](../../com.groupdocs.parser.data/searchresult) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPosition()](#getPosition--) | 获取文档文本中的位置。 |
|
|  | [getText()](#getText--) | 获取文本。 |
|
|  | [getPageIndex()](#getPageIndex--) | 获取找到文本的页索引。 |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | 获取左侧高亮。 |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | 获取右侧高亮。 |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


初始化一个新的 [SearchResult](../../com.groupdocs.parser.data/searchresult) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 位置 | int | 文档文本中的位置。 |
|
|  | 文本 | java.lang.String | 找到的文本。 |
|
|  | pageIndex | java.lang.Integer | 文本所在的页索引。 |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | 左侧高亮。 |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | 右侧高亮。 |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


初始化一个新的 [SearchResult](../../com.groupdocs.parser.data/searchresult) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 位置 | int | 文档文本中的位置。 |
|
|  | 文本 | java.lang.String | 找到的文本。 |
|
|  | pageIndex | java.lang.Integer | 文本所在的页索引。 |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


获取文档文本中的位置。


**Returns:**
int - 搜索结果起始位置的零基索引。

### getText() {#getText--}
```
public String getText()
```


获取文本。


**Returns:**
java.lang.String - 表示找到的文本的字符串值。

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


获取找到文本的页索引。


**Returns:**
java.lang.Integer - 文本所在页的零基索引；如果在整个文档文本上执行搜索，则为 null。

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


获取左侧高亮。


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


获取右侧高亮。


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

