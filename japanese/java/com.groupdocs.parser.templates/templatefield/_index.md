---
title: "TemplateField"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレートのテキストフィールドを提供します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

テンプレートのテキストフィールドを提供します。

テキストフィールドはページ上の位置で定義されます。テキストフィールドを定義する方法は3つあります:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | 新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | 大文字の名前で新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | 大文字の名前で新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | 新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。 |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getPosition()](#getPosition--) | ドキュメントページ上でテンプレートフィールドを見つける方法を示す値を取得します。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | フィールドの位置です。 |
|
|  | 名前 | java.lang.String | フィールド名です。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


大文字の名前で新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | フィールドの位置です。 |
|
|  | 名前 | java.lang.String | フィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


大文字の名前で新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | フィールドの位置です。 |
|
|  | 名前 | java.lang.String | フィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | フィールドの位置です。 |
|
|  | 名前 | java.lang.String | フィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


新しい [TemplateField](../../com.groupdocs.parser.templates/templatefield) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | フィールドの位置です。 |
|
|  | 名前 | java.lang.String | フィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


ドキュメントページ上でテンプレートフィールドを見つける方法を示す値を取得します。


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


指定された係数で全座標をスケーリングした、現在の項目のコピーを作成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
