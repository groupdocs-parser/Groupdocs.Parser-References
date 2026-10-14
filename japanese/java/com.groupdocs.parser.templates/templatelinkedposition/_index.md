---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "リンクされたフィールドを使用するテンプレートフィールド位置を提供します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

リンクされたフィールドを使用するテンプレートフィールド位置を提供します。

以下の例は、請求書番号フィールドが既知である状況のコードを示します
「Invoice number」文字列の右側に配置されている場合、以下のコードが使用されます:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | 新しい [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスのインスタンスを初期化します。 |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | 大文字の名前で新しい [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスのインスタンスを初期化します。 |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | 新しい [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | リンクされたフィールド名を取得します。 |
|
|  | [getSearchArea()](#getSearchArea--) | フィールドが検索される領域のサイズを取得します。 |
|
|  | [isAutoScale()](#isAutoScale--) | リンクされたフィールドサイズで SearchArea がスケーリングされるかどうかを示す値を取得します。 |
|
|  | [getEdges()](#getEdges--) | フィールドが検索されるリンクされたフィールドのエッジを取得します。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


新しい [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | リンクされたフィールドの名前。 |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | フィールドが検索される領域のサイズ。 |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | フィールドが検索されるリンクされたフィールドのエッジ。 |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


大文字の名前で新しい [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | リンクされたフィールドの名前。 |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | フィールドが検索される領域のサイズ。 |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | フィールドが検索されるリンクされたフィールドのエッジ。 |
|
|  | autoScale | boolean | 検索領域がリンクされたフィールドのサイズでスケーリングされるかどうかを示す値です。 |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


新しい [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | リンクされたフィールドの名前。 |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | フィールドが検索される領域のサイズ。 |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | フィールドが検索されるリンクされたフィールドのエッジ。 |
|
|  | autoScale | boolean | 検索領域がリンクされたフィールドのサイズでスケーリングされるかどうかを示す値です。\\ |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


リンクされたフィールド名を取得します。


**Returns:**
java.lang.String - リンクされたフィールド名を表す大文字の文字列値です。

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


フィールドが検索される領域のサイズを取得します。


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


リンクされたフィールドサイズで SearchArea がスケーリングされるかどうかを示す値を取得します。


**Returns:**
java.lang.Boolean - {code true} は、SearchArea がリンクされたフィールドのサイズでスケーリングされる場合; それ以外の場合は false です。

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


フィールドが検索されるリンクされたフィールドのエッジを取得します。


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

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
