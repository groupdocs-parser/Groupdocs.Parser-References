---
title: "Rectangle"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "矩形領域を表します。"
type: docs
weight: 26
url: /ja/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

矩形領域を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | [Rectangle](../../com.groupdocs.parser.data/rectangle) クラスの新しいインスタンスを初期化します。 |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | [Rectangle](../../com.groupdocs.parser.data/rectangle) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getLeft()](#getLeft--) | 矩形領域の左端の x 座標を取得します。 |
|
|  | [getTop()](#getTop--) | 矩形領域の上端の y 座標を取得します。 |
|
|  | [getRight()](#getRight--) | 矩形領域の右端の x 座標を取得します。 |
|
|  | [getBottom()](#getBottom--) | 矩形領域の下端の y 座標を取得します。 |
|
|  | [getPosition()](#getPosition--) | 矩形領域の左上隅の座標を取得します。 |
|
|  | [getSize()](#getSize--) | サイズを取得します。 |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


[Rectangle](../../com.groupdocs.parser.data/rectangle) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 左 | double | 矩形領域の左端の x 座標。 |
|
|  | 上 | double | 矩形領域の上端の y 座標。 |
|
|  | 右 | double | 矩形領域の右端の x 座標。 |
|
|  | 下 | double | 矩形領域の下端の y 座標。 |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


[Rectangle](../../com.groupdocs.parser.data/rectangle) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | 矩形領域の左上隅の座標。 |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | 矩形領域のサイズ。 |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


矩形領域の左端の x 座標を取得します。


**Returns:**
double - 矩形領域の左端の x 座標を表す double 値。

### getTop() {#getTop--}
```
public double getTop()
```


矩形領域の上端の y 座標を取得します。


**Returns:**
double - 矩形領域の上端の y 座標を表す double 値。

### getRight() {#getRight--}
```
public double getRight()
```


矩形領域の右端の x 座標を取得します。


**Returns:**
double - 矩形領域の右端の x 座標を表す double 値。

### getBottom() {#getBottom--}
```
public double getBottom()
```


矩形領域の下端の y 座標を取得します。


**Returns:**
double - 矩形領域の下端の y 座標を表す double 値。

### getPosition() {#getPosition--}
```
public Point getPosition()
```


矩形領域の左上隅の座標を取得します。


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


サイズを取得します。


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
