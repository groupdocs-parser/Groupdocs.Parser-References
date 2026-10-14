---
title: "TextOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テキスト抽出に使用されるオプションを提供します。"
type: docs
weight: 37
url: /ja/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

テキスト抽出に使用されるオプションを提供します。

[TextOptions](../../com.groupdocs.parser.options/textoptions) クラスのインスタンスは、[Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-) のパラメータとして使用されます。
および [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) メソッドです。使用例はそちらをご覧ください。

テキスト抽出の生モードを指定するために使用されます。このモードのテキストは正確ではない形で抽出されます。
標準モードよりも高速ですが、正確ではありません。生モードがドキュメント形式をサポートしない場合、
このパラメータは無視され、標準モードが使用されます。

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR 使用オプション付きで初期化します。 |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | [TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR オプションを設定できるように初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | 生モードが使用されているかどうかを示す値を取得します。 |
|
|  | [isUseOcr()](#isUseOcr--) | OCR コネクタがテキスト抽出に使用されているかどうかを示す値を取得します。 |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR 機能の追加オプションを取得します。 |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | 抽出されたテキストに注釈が含まれるかどうかを示す値を取得します。 |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | 抽出されたテキストに注釈が含まれるかどうかを示す値を設定します。 |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 生モードが使用されているかどうかを示す値。 |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR 使用オプション付きで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 生モードが使用されているかどうかを示す値。 |
|
|  | useOcr | boolean | OCR 機能がテキスト抽出に使用されているかどうかを示す値です。 |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


[TextOptions](../../com.groupdocs.parser.options/textoptions) クラスの新しいインスタンスを、OCR オプションを設定できるように初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | 生モードが使用されているかどうかを示す値。 |
|
|  | useOcr | boolean | OCR 機能がテキスト抽出に使用されているかどうかを示す値です。 |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR 機能の追加オプションです。 |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


生モードが使用されているかどうかを示す値を取得します。


**Returns:**
boolean - 生モードが使用されている場合は true、そうでない場合は false。

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


抽出されたテキストに注釈が含まれるかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 注釈が含まれる場合は true、そうでない場合は false。

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


抽出されたテキストに注釈が含まれるかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | includeAnnotations | boolean | 抽出されたテキストに注釈を含める場合は true。 |
|

