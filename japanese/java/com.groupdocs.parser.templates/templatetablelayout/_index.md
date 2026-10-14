---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレートテーブルレイアウトを提供します。このレイアウトは class によってテーブル位置を定義するために使用されます。"
type: docs
weight: 21
url: /ja/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

テンプレートテーブルレイアウトを提供します。このレイアウトは [TemplateTable](../../com.groupdocs.parser.templates/templatetable) クラスによってテーブル位置を定義するために使用されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | 新しいインスタンスを初期化します [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) クラス。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | テーブルを含む矩形領域を取得します。 |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | テーブルの列区切りを取得します。 |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | テーブルの行区切りを取得します。 |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | 同じサイズ、区切り、位置を持つ新しいレイアウトをポイント単位で作成します。 |
|
|  | [scale(double factor)](#scale-double-) | このレイアウトのコピーを作成し、すべての座標を指定された factor でスケーリングします。 |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


新しいインスタンスを初期化します [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) クラス。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | テーブルの列区切りです。 |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | テーブルの行区切りです。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


テーブルを含む矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


テーブルの列区切りを取得します。


**Returns:**
java.util.List<java.lang.Double> - テーブルの列区切りの x 座標を表す double 値のコレクションです。

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


テーブルの行区切りを取得します。


**Returns:**
java.util.List<java.lang.Double> - テーブルの行区切りの y 座標を表す double 値のコレクションです。

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


同じサイズ、区切り、位置を持つ新しいレイアウトをポイント単位で作成します。

この機能により Table Layout を移動できます。

例えば、ドキュメントの各ページにテーブルがある（またはページにテーブルがあるドキュメントのセット）場合です。
これらのテーブルは位置と内容が異なりますが、列と行は同じです。この場合、ユーザーは
(0, 0) に一度 [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) オブジェクトを定義し、その後、確定テーブルの位置へ移動できます。

テーブルの位置がページ上の他のオブジェクトに依存する場合、ユーザーは [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) オブジェクトを定義できます。
テンプレートドキュメントに基づき、アンカーオブジェクトに従って移動します。例えば、これがサマリーテーブルの場合
そしてそれに続いて詳細テーブルがあり（行数が異なる場合があります）。この場合、ユーザーは定義できます
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
このメソッドは現在のオブジェクトのコピーを返します。ユーザーは任意の座標を渡すことができます。
（負の値でも構いません - その場合レイアウトは左/上に移動します）。

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | 新しいレイアウトの位置です。 |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


このレイアウトのコピーを作成し、すべての座標を指定された factor でスケーリングします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | factor | double | スケーリング係数です。 |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

