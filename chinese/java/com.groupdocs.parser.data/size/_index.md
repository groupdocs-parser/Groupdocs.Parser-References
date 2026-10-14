---
title: "Size"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示一个尺寸。"
type: docs
weight: 28
url: /zh/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

表示一个尺寸。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | 初始化 [Size](../../com.groupdocs.parser.data/size) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 获取宽度。 |
|
|  | [getHeight()](#getHeight--) | 获取高度。 |
|
|  | [isEmpty()](#isEmpty--) | 获取指示大小是否为空的值。 |
|
|  | [parse(String s)](#parse-java.lang.String-) | 将大小的字符串表示转换为其对应的类实例。 |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


初始化 [Size](../../com.groupdocs.parser.data/size) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 宽度 | double | 以像素为单位的宽度。 |
|
|  | 高度 | double | 以像素为单位的高度。 |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


获取宽度。


**Returns:**
double - 表示像素宽度的 double 值。

### getHeight() {#getHeight--}
```
public double getHeight()
```


获取高度。


**Returns:**
double - 表示像素高度的 double 值。

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


获取指示大小是否为空的值。


**Returns:**
boolean - 如果宽度和高度为零则为 true；否则为 false。

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


将大小的字符串表示转换为其对应的类实例。返回值指示转换是成功还是失败。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | s | java.lang.String | 包含要转换的大小的字符串。 |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
