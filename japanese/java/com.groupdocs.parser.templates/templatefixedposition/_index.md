---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "矩形領域で定義されるテンプレートフィールド位置を提供します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

矩形領域で定義されるテンプレートフィールド位置を提供します。

これはフィールド位置を定義する最も簡単な方法です。ページ上でフィールドを囲む長方形領域を設定する必要があります。
フィールドの値です。長方形領域内に含まれる（部分的であっても）すべてのテキストが値として抽出されます:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | 新しい [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | テンプレートフィールドを含む長方形領域を取得します。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


新しい [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テンプレートフィールドを含む長方形領域です。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


テンプレートフィールドを含む長方形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


現在の位置のコピーを作成し、すべての座標を指定された factor でスケーリングします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
