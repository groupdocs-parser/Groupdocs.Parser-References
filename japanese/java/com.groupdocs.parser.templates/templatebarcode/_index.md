---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレートのバーコードフィールドを提供します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

テンプレートのバーコードフィールドを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | 新しい [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスのインスタンスを初期化します。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | UPPER CASE 名で [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | UPPER CASE 名で [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスの新しいインスタンスを初期化します。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | 新しい [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスのインスタンスを初期化します。 |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | 新しい [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | テンプレートバーコードフィールドを含む矩形領域を取得します。 |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


新しい [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テンプレートバーコードフィールドを含む矩形領域です。 |
|
|  | 名前 | java.lang.String | バーコードフィールド名です。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


UPPER CASE 名で [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テンプレートバーコードフィールドを含む矩形領域です。 |
|
|  | 名前 | java.lang.String | バーコードフィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


UPPER CASE 名で [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テンプレートバーコードフィールドを含む矩形領域です。 |
|
|  | 名前 | java.lang.String | バーコードフィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


新しい [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テンプレートバーコードフィールドを含む矩形領域です。 |
|
|  | 名前 | java.lang.String | バーコードフィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


新しい [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テンプレートバーコードフィールドを含む矩形領域です。 |
|
|  | 名前 | java.lang.String | バーコードフィールド名です。 |
|
|  | pageIndex | java.lang.Integer | テンプレート項目が配置されているページのインデックスを表す整数値です。テンプレート項目が任意のページにある場合は null です。 |
|
|  | pageWidth | java.lang.Double | テンプレート項目の作成に使用されたページの幅。 |
|
|  | useUpperCaseName | boolean | 名前が大文字に変換されるかどうかを示す値。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


テンプレートバーコードフィールドを含む矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

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
