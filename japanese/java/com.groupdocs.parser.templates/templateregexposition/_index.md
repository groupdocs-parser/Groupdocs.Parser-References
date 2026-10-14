---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "正規表現を使用するテンプレートフィールド位置を提供します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

正規表現を使用するテンプレートフィールド位置を提供します。

次の例は、文書に "Invoice Number INV-12345" が含まれる場合の状況を示しています。
その場合、テンプレートフィールドは以下のように定義できます：

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

この場合、値として文字列全体が抽出されます。文字列の一部だけを抽出するには
正規表現グループ "value" が使用されます:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

この場合、値として "INV-3337" 文字列が抽出されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | 新しいインスタンスを初期化します [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) クラス。 |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | 新しいインスタンスを初期化します [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) クラス。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getExpression()](#getExpression--) | 正規表現を取得します。 |
|
|  | [isMatchCase()](#isMatchCase--) | テキストの大文字小文字が無視されないかどうかを示す値を取得します。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


新しいインスタンスを初期化します [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) クラス。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


新しいインスタンスを初期化します [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) クラス。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


正規表現を取得します。


**Returns:**
java.lang.String - 正規表現を表す文字列です。

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


テキストの大文字小文字が無視されないかどうかを示す値を取得します。


**Returns:**
boolean -  true  テキストケースが無視されていない場合; それ以外は  false です。

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
