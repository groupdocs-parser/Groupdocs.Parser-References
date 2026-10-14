---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于 OCR 事件的处理程序。"
type: docs
weight: 26
url: /zh/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

提供用于 OCR 事件的处理程序。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | 初始化 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | 获取警告消息列表。 |
|
|  | [hasWarnings()](#hasWarnings--) | 获取指示警告列表是否非空的值。 |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | 返回具有 pageIndex 页的警告消息列表。 |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | 设置该页的警告消息。 |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


初始化 [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) 类的新实例。


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


获取警告消息列表。


**Returns:**
java.util.List<java.lang.String> - 所有页面的警告消息列表。

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


获取指示警告列表是否非空的值。


**Returns:**
boolean -  true  如果警告列表非空；否则，  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


返回具有 pageIndex 页的警告消息列表。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|

**Returns:**
java.util.List<java.lang.String> - 该页的警告消息列表；如果该页没有警告消息，则为空列表。

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


设置该页的警告消息。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 从零开始的页面索引。 |
|
|  | warnings | java.lang.Iterable<java.lang.String> | 该页的警告消息列表。 |
|

