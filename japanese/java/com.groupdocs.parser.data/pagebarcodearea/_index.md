---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート解析機能でバーコード値を表すために使用されるページバーコード領域を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

テンプレート解析機能でバーコード値を表すために使用されるページバーコード領域を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getValue()](#getValue--) | バーコードの値を取得します。 |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | バーコードタイプの名前を取得します。 |
|
|  | [getConfidence()](#getConfidence--) | 解析されたバーコードの信頼度レベルを取得します。 |
|
|  | [getAngle()](#getAngle--) | バーコードの角度を取得します。 |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


[PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | バーコードの値です。 |
|
|  | codeTypeName | java.lang.String | バーコードのタイプ名です。 |
|
|  | confidence | int | 解析されたバーコードの信頼度レベルです。 |
|
|  | angle | double | バーコードの角度です。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | バーコード領域を含むページです。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | バーコード領域を含む矩形領域です。 |
|

### getValue() {#getValue--}
```
public String getValue()
```


バーコードの値を取得します。


**Returns:**
java.lang.String - バーコードページ領域の値を表す文字列です。

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


バーコードタイプの名前を取得します。


**Returns:**
java.lang.String - バーコードのタイプ名を表す文字列です。

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


解析されたバーコードの信頼度レベルを取得します。


**Returns:**
int - 解析されたバーコードの信頼度 (0-100) を表す整数値です。

### getAngle() {#getAngle--}
```
public double getAngle()
```


バーコードの角度を取得します。


**Returns:**
double - バーコードの角度 (0-360) を表す実数値です。

