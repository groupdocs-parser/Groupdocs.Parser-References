---
title: "Point"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "点を表します。"
type: docs
weight: 25
url: /ja/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

点を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | [Point](../../com.groupdocs.parser.data/point) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getX()](#getX--) | X 座標を取得します。 |
|
|  | [getY()](#getY--) | Y 座標を取得します。 |
|
|  | [parse(String s)](#parse-java.lang.String-) | ポイントの文字列表現をクラスの等価オブジェクトに変換します。 |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


[Point](../../com.groupdocs.parser.data/point) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | x | double | X 座標。 |
|
|  | y | double | Y 座標。 |
|

### getX() {#getX--}
```
public double getX()
```


X 座標を取得します。


**Returns:**
double - X 座標を表す double 値。

### getY() {#getY--}
```
public double getY()
```


Y 座標を取得します。


**Returns:**
double - Y 座標を表す double 値。

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


ポイントの文字列表現をクラスの等価オブジェクトに変換します。戻り値は変換が成功したか失敗したかを示します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | s | java.lang.String | 変換対象のポイントを含む文字列。 |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
