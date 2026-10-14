---
title: "点"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示一个点。"
type: docs
weight: 25
url: /zh/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

表示一个点。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | 初始化 [Point](../../com.groupdocs.parser.data/point) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getX()](#getX--) | 获取 x 坐标。 |
|
|  | [getY()](#getY--) | 获取 y 坐标。 |
|
|  | [parse(String s)](#parse-java.lang.String-) | 将点的字符串表示转换为其类等价形式。 |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


初始化 [Point](../../com.groupdocs.parser.data/point) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | x | double | x 坐标。 |
|
|  | y | double | y 坐标。 |
|

### getX() {#getX--}
```
public double getX()
```


获取 x 坐标。


**Returns:**
double - 表示 x 坐标的 double 值。

### getY() {#getY--}
```
public double getY()
```


获取 y 坐标。


**Returns:**
double - 表示 y 坐标的 double 值。

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


将点的字符串表示转换为其类等价形式。返回值指示转换是成功还是失败。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | s | java.lang.String | 包含要转换的点的字符串。 |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
