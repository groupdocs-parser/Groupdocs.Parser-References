---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ページテキスト領域抽出に使用されるオプションを提供します。"
type: docs
weight: 32
url: /ja/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object、[com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

ページテキスト領域抽出に使用されるオプションを提供します。

インスタンス [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスは、[Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-) のパラメータとして使用されます。
および [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) メソッドです。使用例をご覧ください。

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | デフォルト値で [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR 使用オプション付きで初期化します。 |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR オプションを設定できるように初期化します。 |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | 正規表現を使用して [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | 正規表現と矩形領域を使用して [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | 正規表現、矩形領域、および無視される境界のサイズを使用して [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | 無視される境界のサイズを使用して [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getExpression()](#getExpression--) | 正規表現を取得します。 |
|
|  | [isMatchCase()](#isMatchCase--) | テキストの大文字小文字が無視されないかどうかを示す値を取得します。 |
|
|  | [isUniteSegments()](#isUniteSegments--) | セグメントが結合されているかどうかを示す値を取得します。 |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | テキストの書式設定が無視されるかどうかを示す値を取得します。 |
|
|  | [isUseOcr()](#isUseOcr--) | OCR コネクタがテキスト抽出に使用されているかどうかを示す値を取得します。 |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR 機能の追加オプションを取得します。 |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


デフォルト値で [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR 使用オプション付きで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | useOcr | boolean | OCR 機能がテキスト抽出に使用されているかどうかを示す値です。 |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR オプションを設定できるように初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | useOcr | boolean | OCR 機能がテキスト抽出に使用されているかどうかを示す値です。 |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 機能の追加オプションです。 |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


正規表現で [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。他のオプションはデフォルトで設定されます（詳細は備考をご参照ください）。

以下のプロパティはデフォルト値を持ちます：

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


正規表現と矩形領域で [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。他のオプションはデフォルトで設定されます（詳細は備考をご参照ください）。

以下のプロパティはデフォルト値を持ちます：

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ領域を含む矩形領域です。 |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


正規表現、矩形領域、および無視される境界のサイズで [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。他のオプションはデフォルトで設定されます（詳細は備考をご参照ください）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ領域を含む矩形領域です。 |
|
|  | rectangleTolerance | double | 矩形領域でキャプチャされる際に無視される境界のサイズです。テキスト項目の高さの割合で測定されます。 |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


[PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | uniteSegments | boolean | セグメントが結合されているかどうかを示す値です。 |
|
|  | ignoreFormatting | boolean | テキスト書式が無視されているかどうかを示す値です。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ領域を含む矩形領域です。 |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


無視される境界のサイズを使用して [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | expression | java.lang.String | 正規表現です。 |
|
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | uniteSegments | boolean | セグメントが結合されているかどうかを示す値です。 |
|
|  | ignoreFormatting | boolean | テキスト書式が無視されているかどうかを示す値です。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ領域を含む矩形領域です。 |
|
|  | rectangleTolerance | double | 矩形領域でキャプチャされる際に無視される境界のサイズです。テキスト項目の高さの割合で測定されます。 |
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

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


セグメントが結合されているかどうかを示す値を取得します。


**Returns:**
boolean - {code true} セグメントが結合されている場合; それ以外は {code false} です。

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


テキストの書式設定が無視されるかどうかを示す値を取得します。


**Returns:**
boolean -  true  テキスト書式が無視されている場合; それ以外は  false です。

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


OCR コネクタがテキスト抽出に使用されているかどうかを示す値を取得します。


**Returns:**
boolean - OCR 機能が使用されている場合は true、そうでない場合は false。

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


OCR 機能の追加オプションを取得します。


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

