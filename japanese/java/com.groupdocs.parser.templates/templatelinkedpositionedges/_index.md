---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テキストフィールドが検索されるリンクされたフィールドのエッジを提供します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

テキストフィールドが検索されるリンクフィールドのエッジを提供します。[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) は [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) クラスで使用されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | インスタンスが空かどうかを示す値を取得します。 |
|
|  | [isLeft()](#isLeft--) | リンクフィールドの左側からフィールドが検索されるかどうかを示す値を取得します。 |
|
|  | [isTop()](#isTop--) | リンクフィールドの上側からフィールドが検索されるかどうかを示す値を取得します。 |
|
|  | [isRight()](#isRight--) | リンクフィールドの右側からフィールドが検索されるかどうかを示す値を取得します。 |
|
|  | [isBottom()](#isBottom--) | リンクフィールドの下側からフィールドが検索されるかどうかを示す値を取得します。 |
|
|  | [parse(String s)](#parse-java.lang.String-) | エッジの文字列表現をクラスの等価オブジェクトに変換します。 |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 左 | boolean | リンクフィールドの左側からフィールドが検索されるかどうかを示す値です。 |
|
|  | 上 | boolean | リンクフィールドの上側からフィールドが検索されるかどうかを示す値です。 |
|
|  | 右 | boolean | リンクフィールドの右側からフィールドが検索されるかどうかを示す値です。 |
|
|  | 下 | boolean | リンクされたフィールドの下からフィールドが検索されるかどうかを示す値。 |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


インスタンスが空かどうかを示す値を取得します。


**Returns:**
boolean - インスタンスが空の場合は true (すべてのフィールドが false)；それ以外は false。

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


リンクフィールドの左側からフィールドが検索されるかどうかを示す値を取得します。


**Returns:**
boolean - リンクされたフィールドの左からフィールドが検索される場合は true；それ以外は false。

### isTop() {#isTop--}
```
public boolean isTop()
```


リンクフィールドの上側からフィールドが検索されるかどうかを示す値を取得します。


**Returns:**
boolean - リンクされたフィールドの上からフィールドが検索される場合は true；それ以外は false。

### isRight() {#isRight--}
```
public boolean isRight()
```


リンクフィールドの右側からフィールドが検索されるかどうかを示す値を取得します。


**Returns:**
boolean - リンクされたフィールドの右からフィールドが検索される場合は true；それ以外は false。

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


リンクフィールドの下側からフィールドが検索されるかどうかを示す値を取得します。


**Returns:**
boolean - リンクされたフィールドの下からフィールドが検索される場合は true；それ以外は false。

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


エッジの文字列表現をクラスの等価オブジェクトに変換します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | s | java.lang.String | 変換するエッジを含む文字列。 |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
