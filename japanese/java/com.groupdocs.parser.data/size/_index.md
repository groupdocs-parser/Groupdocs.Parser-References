---
title: "Size"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "サイズを表します。"
type: docs
weight: 28
url: /ja/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

サイズを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | 新しい [Size](../../com.groupdocs.parser.data/size) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 幅を取得します。 |
|
|  | [getHeight()](#getHeight--) | 高さを取得します。 |
|
|  | [isEmpty()](#isEmpty--) | サイズが空かどうかを示す値を取得します。 |
|
|  | [parse(String s)](#parse-java.lang.String-) | サイズの文字列表現をクラスの等価オブジェクトに変換します。 |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


新しい [Size](../../com.groupdocs.parser.data/size) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | width | double | ピクセル単位の幅です。 |
|
|  | height | double | ピクセル単位の高さです。 |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


幅を取得します。


**Returns:**
double - ピクセル単位の幅を表す double 値です。

### getHeight() {#getHeight--}
```
public double getHeight()
```


高さを取得します。


**Returns:**
double - ピクセル単位の高さを表す double 値です。

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


サイズが空かどうかを示す値を取得します。


**Returns:**
boolean - 幅と高さがゼロの場合は true、そうでない場合は false です。

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


サイズの文字列表現をクラスの等価オブジェクトに変換します。戻り値は変換が成功したか失敗したかを示します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | s | java.lang.String | 変換対象のサイズを含む文字列です。 |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
