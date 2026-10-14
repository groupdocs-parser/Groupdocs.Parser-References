---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テーブル検出アルゴリズムのパラメータを提供します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

テーブル検出アルゴリズムのパラメータを提供します。

テーブルを検出するためのアルゴリズムは2つあります：

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

アルゴリズムがテーブルを検出できない、または正確に検出できない場合、[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) クラスが使用されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | テーブルを含む矩形領域を取得します。 |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | テーブルの列区切りを取得します。 |
|
|  | [hasMergedCells()](#hasMergedCells--) | テーブルに結合セルがあるかどうかを示す値を取得します。 |
|
|  | [getMinRowCount()](#getMinRowCount--) | テーブルの行数の最小値を取得します。 |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | テーブルの列数の最小値を取得します。 |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | テーブルの列間の最小スペースを取得します。 |
|
|  | [scale(double factor)](#scale-double-) | これらのパラメータのコピーを作成し、すべての座標を指定された係数でスケーリングします。 |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テーブルを含む矩形領域。 |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | テーブルの列区切りです。 |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テーブルを含む矩形領域。 |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | テーブルの列区切りです。 |
|
|  | mergedCells | java.lang.Boolean | テーブルに結合セルがあるかどうかを示す値。 |
|
|  | minRowCount | java.lang.Integer | テーブルの行数の最小値。 |
|
|  | minColumnCount | java.lang.Integer | テーブルの列数の最小値。 |
|
|  | minVerticalSpace | java.lang.Integer | テーブル列間の最小スペースです。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


テーブルを含む矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


テーブルの列区切りを取得します。


**Returns:**
java.util.List<java.lang.Double> - テーブル列の区切りの x 座標を表す double 値のコレクションです。設定されていない場合は  null  です。

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


テーブルに結合セルがあるかどうかを示す値を取得します。


**Returns:**
java.lang.Boolean - テーブルに結合されたセルがある場合は  true  、それ以外の場合は  false  です。設定されていない場合は  null  です。

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


テーブルの行数の最小値を取得します。


**Returns:**
java.lang.Integer - テーブル行の最小数を表す整数値です。設定されていない場合は  null  です。

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


テーブルの列数の最小値を取得します。


**Returns:**
java.lang.Integer - テーブル列の最小数を表す整数値です。設定されていない場合は  null  です。

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


テーブルの列間の最小スペースを取得します。


**Returns:**
java.lang.Integer - テーブル列間の最小スペースを表す整数値です。設定されていない場合は  null  です。

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


これらのパラメータのコピーを作成し、すべての座標を指定された係数でスケーリングします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | factor | double | スケーリング係数です。 |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

