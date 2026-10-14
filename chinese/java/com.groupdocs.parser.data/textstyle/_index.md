---
title: "TextStyle"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示文本的样式，例如字体名称、字体大小等。"
type: docs
weight: 30
url: /zh/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

表示文本的样式，例如字体名称、字体大小等。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | 初始化 [TextStyle](../../com.groupdocs.parser.data/textstyle) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getName()](#getName--) | 获取样式名称。 |
|
|  | [getFontName()](#getFontName--) | 获取字体名称。 |
|
|  | [getFontSize()](#getFontSize--) | 获取字体大小。 |
|
|  | [isBold()](#isBold--) | 获取指示字体是否加粗的值。 |
|
|  | [isItalic()](#isItalic--) | 获取指示字体是否斜体的值。 |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


初始化 [TextStyle](../../com.groupdocs.parser.data/textstyle) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 名称 | java.lang.String | 样式的名称。 |
|
|  | fontName | java.lang.String | 字体的名称。 |
|
|  | fontSize | double | 字体的大小。 |
|
|  | bold | boolean | 指示字体是否加粗的值。 |
|
|  | italic | boolean | 指示字体是否斜体的值。 |
|

### getName() {#getName--}
```
public String getName()
```


获取样式名称。


**Returns:**
java.lang.String - 表示样式名称的字符串值。

### getFontName() {#getFontName--}
```
public String getFontName()
```


获取字体名称。


**Returns:**
java.lang.String - 表示字体名称的字符串值。

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


获取字体大小。


**Returns:**
double - 表示字体大小的 double 值。

### isBold() {#isBold--}
```
public boolean isBold()
```


获取指示字体是否加粗的值。


**Returns:**
boolean -  true  如果字体为粗体；否则，  false 。

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


获取指示字体是否斜体的值。


**Returns:**
boolean -  true  如果字体为斜体；否则，  false 。

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
