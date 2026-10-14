---
title: "TextReader"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示能够读取字符序列的读取器。"
type: docs
weight: 29
url: /zh/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

表示能够读取字符序列的读取器。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | 从文本读取器读取一行字符，并将数据作为字符串返回。 |
|
|  | [readToEnd()](#readToEnd--) | 读取从当前位置到文本读取器末尾的所有字符，并将它们作为一个字符串返回。 |
|
|  | [dispose()](#dispose--) | 释放由 [TextReader](../../com.groupdocs.parser.data/textreader) 对象使用的所有资源。 |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


从文本读取器读取一行字符，并将数据作为字符串返回。


**Returns:**
java.lang.String - 来自读取器的下一行，如果已读取完所有字符，则为  null  。

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


读取从当前位置到文本读取器末尾的所有字符，并将它们作为一个字符串返回。


**Returns:**
java.lang.String - 包含从当前位置到文本读取器末尾的所有字符的字符串。

### dispose() {#dispose--}
```
public void dispose()
```


释放由 [TextReader](../../com.groupdocs.parser.data/textreader) 对象使用的所有资源。


