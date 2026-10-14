---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "OCR機能を提供します。"
type: docs
weight: 25
url: /ja/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

OCR機能を提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | 新しいインスタンスの [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) クラスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | テキスト抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | テキスト領域の抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | imageStream ストリームからテキストを認識します。 |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | imageStream ストリームからテキスト領域を認識します。 |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


新しいインスタンスの [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) クラスを初期化します。


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


テキスト抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean - テキスト抽出がサポートされている場合は true、そうでない場合は false。

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


テキスト領域の抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean - テキスト抽出領域がサポートされている場合は true、そうでない場合は false。

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


imageStream ストリームからテキストを認識します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | ドキュメントページの画像表現です。 |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR オプションです。 |
|

**Returns:**
java.lang.String - 認識されたテキストを表す文字列です。テキスト認識がサポートされていない場合は null。

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


imageStream ストリームからテキスト領域を認識します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | ドキュメントページの画像表現です。 |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | ドキュメントページのサイズです。 |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR オプションです。 |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。テキスト領域の認識がサポートされていない場合は null。

