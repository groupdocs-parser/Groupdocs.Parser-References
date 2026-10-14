---
title: "OcrOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "OCRコネクタに使用されるオプションを提供します。"
type: docs
weight: 27
url: /ja/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

OCRコネクタに使用されるオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | デフォルト値で [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | 矩形領域を指定して [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | ページプレビューオプションを使用して [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) オブジェクトとともに [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | 矩形領域と [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) オブジェクトを指定して [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | テキスト認識に使用されるページ領域を制限する矩形領域を取得します。 |
|
|  | [getHandler()](#getHandler--) | OCR イベントを捕捉するイベントハンドラを取得します。 |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | スペルチェッカーが使用されているかどうかを示す値を取得します。 |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | OCR エンジンに供給されるページをレンダリングするために使用されるページプレビューオプションを取得します。 |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | OCR エンジンに供給されるページをレンダリングするために使用されるページプレビューオプションを設定します。 |
|
|  | [getLanguage()](#getLanguage--) | 光学文字認識に使用される言語を取得します。 |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | 光学文字認識に使用される言語を設定します。 |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | テキスト認識に使用されるページ領域を制限する矩形領域を設定します。 |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | OCR イベントを捕捉するイベントハンドラを設定します。 |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | スペルチェッカーが使用されているかどうかを示す値を設定します。 |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


デフォルト値で [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


矩形領域を指定して [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テキスト認識に使用されるページ領域を制限する矩形領域です。 |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


ページプレビューオプションを使用して [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | OCR エンジンに供給されるページプレビューをレンダリングするために使用されるオプションです。 |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) オブジェクトとともに [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR イベントを捕捉するための [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) のインスタンスです。 |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


矩形領域と [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) オブジェクトを指定して [OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テキスト認識に使用されるページ領域を制限する矩形領域です。 |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR イベントを捕捉するための [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) のインスタンスです。 |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


[OcrOptions](../../com.groupdocs.parser.options/ocroptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テキスト認識に使用されるページ領域を制限する矩形領域です。 |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR イベントを捕捉するための [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) のインスタンスです。 |
|
|  | useSpellCheker | boolean | スペルチェッカーが使用されているかどうかを示す値です。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


テキスト認識に使用されるページ領域を制限する矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


OCR イベントを捕捉するイベントハンドラを取得します。


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


スペルチェッカーが使用されているかどうかを示す値を取得します。


**Returns:**
boolean - スペルチェッカーが使用されている場合は true、そうでない場合は false。

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


OCR エンジンに供給されるページをレンダリングするために使用されるページプレビューオプションを取得します。


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


OCR エンジンに供給されるページをレンダリングするために使用されるページプレビューオプションを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | ページプレビューオプションです。 |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


光学文字認識に使用される言語を取得します。


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


光学文字認識に使用される言語を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | [Language](../../com.groupdocs.parser.options/language) 列挙値です。 |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


テキスト認識に使用されるページ領域を制限する矩形領域を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 矩形、または  null  を使用してページ全体をスキャンします。 |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


OCR イベントを捕捉するイベントハンドラを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | イベントハンドラです。 |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


スペルチェッカーが使用されているかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  を使用してスペルチェックを有効にします。 |
|

