---
title: "Rectangle"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示一个矩形区域。"
type: docs
weight: 26
url: /zh/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

表示一个矩形区域。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | 初始化 [Rectangle](../../com.groupdocs.parser.data/rectangle) 类的新实例。 |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | 初始化 [Rectangle](../../com.groupdocs.parser.data/rectangle) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getLeft()](#getLeft--) | 获取矩形区域左边缘的 x 坐标。 |
|
|  | [getTop()](#getTop--) | 获取矩形区域上边缘的 y 坐标。 |
|
|  | [getRight()](#getRight--) | 获取矩形区域右边缘的 x 坐标。 |
|
|  | [getBottom()](#getBottom--) | 获取矩形区域下边缘的 y 坐标。 |
|
|  | [getPosition()](#getPosition--) | 获取矩形区域左上角的坐标。 |
|
|  | [getSize()](#getSize--) | 获取大小。 |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


初始化 [Rectangle](../../com.groupdocs.parser.data/rectangle) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 左 | double | 矩形区域左边缘的 x 坐标。 |
|
|  | 上 | double | 矩形区域上边缘的 y 坐标。 |
|
|  | 右 | double | 矩形区域右边缘的 x 坐标。 |
|
|  | 底部 | double | 矩形区域底部边缘的 y 坐标。 |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


初始化 [Rectangle](../../com.groupdocs.parser.data/rectangle) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | 矩形区域左上角的坐标。 |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | 矩形区域的大小。 |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


获取矩形区域左边缘的 x 坐标。


**Returns:**
double - 表示矩形区域左边缘的 x 坐标的 double 值。

### getTop() {#getTop--}
```
public double getTop()
```


获取矩形区域上边缘的 y 坐标。


**Returns:**
double - 表示矩形区域上边缘的 y 坐标的 double 值。

### getRight() {#getRight--}
```
public double getRight()
```


获取矩形区域右边缘的 x 坐标。


**Returns:**
double - 表示矩形区域右边缘的 x 坐标的 double 值。

### getBottom() {#getBottom--}
```
public double getBottom()
```


获取矩形区域下边缘的 y 坐标。


**Returns:**
double - 表示矩形区域底部边缘的 y 坐标的 double 值。

### getPosition() {#getPosition--}
```
public Point getPosition()
```


获取矩形区域左上角的坐标。


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


获取大小。


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
