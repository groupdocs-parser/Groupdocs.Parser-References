---
title: "機能"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "サポートされている機能の一覧を表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

サポートされている機能のリストを表します。ドキュメントに対してどの機能がサポートされているか、されていないかの情報を取得できます。

このクラスのインスタンスは [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) プロパティとして使用されます。使用例はそちらをご覧ください。

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Features()](#Features--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | 機能がサポートされているかどうかを示す値を返します。 |
|
|  | [isText()](#isText--) | テキスト抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isTextPage()](#isTextPage--) | テキストページ抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isFormattedText()](#isFormattedText--) | 書式付きテキスト抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | 書式付きテキストページ抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isSearch()](#isSearch--) | テキスト検索がサポートされているかどうかを示す値を取得します。 |
|
|  | [isHighlight()](#isHighlight--) | ハイライト抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isBarcodes()](#isBarcodes--) | バーコード抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isToc()](#isToc--) | 目次抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isMetadata()](#isMetadata--) | メタデータ抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isContainer()](#isContainer--) | コンテナ抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isTextAreas()](#isTextAreas--) | テキスト領域抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isStructure()](#isStructure--) | テキスト構造抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isImages()](#isImages--) | 画像抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isHyperlinks()](#isHyperlinks--) | ハイパーリンク抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isTables()](#isTables--) | テーブル抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isAnnotations()](#isAnnotations--) | 注釈抽出がサポートされているかどうかを示す値を取得します。 |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | テンプレートによる解析がサポートされているかどうかを示す値を取得します。 |
|
|  | [isParseForm()](#isParseForm--) | フォーム解析がサポートされているかどうかを示す値を取得します。 |
|
|  | [isPreview()](#isPreview--) | プレビュー生成がサポートされているかどうかを示す値を取得します。 |
|
|  | [isPagePreview()](#isPagePreview--) | ページプレビュー生成がサポートされているかどうかを示す値を取得します。 |
|
|  | [isOcr()](#isOcr--) | OCR 機能がサポートされているかどうかを示す値を取得します。 |
|
|  | [isWorksheet()](#isWorksheet--) | ワークシート抽出がサポートされているかどうかを示す値を取得します。 |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


機能がサポートされているかどうかを示す値を返します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | featureName | java.lang.String | 機能名です。 |
|

**Returns:**
boolean -  true  if 機能がサポートされている場合; それ以外の場合は false .

### isText() {#isText--}
```
public boolean isText()
```


テキスト抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テキスト抽出がサポートされている場合; それ以外の場合は false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


テキストページ抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テキストページ抽出がサポートされている場合; それ以外の場合は false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


書式付きテキスト抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if 書式付きテキスト抽出がサポートされている場合; それ以外の場合は false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


書式付きテキストページ抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if 書式付きテキストページがサポートされている場合; それ以外の場合は false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


テキスト検索がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テキスト検索がサポートされている場合; それ以外の場合は false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


ハイライト抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if ハイライト抽出がサポートされている場合; それ以外の場合は false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


バーコード抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if バーコード抽出がサポートされている場合; それ以外の場合は false .

### isToc() {#isToc--}
```
public boolean isToc()
```


目次抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if 目次抽出がサポートされている場合; それ以外の場合は false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


メタデータ抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if メタデータ抽出がサポートされている場合; それ以外の場合は false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


コンテナ抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if コンテナ抽出がサポートされている場合; それ以外の場合は false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


テキスト領域抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テキスト領域抽出がサポートされている場合; それ以外の場合は false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


テキスト構造抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テキスト構造抽出がサポートされている場合; それ以外の場合は false .

### isImages() {#isImages--}
```
public boolean isImages()
```


画像抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if 画像抽出がサポートされている場合; それ以外の場合は false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


ハイパーリンク抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if ハイパーリンク抽出がサポートされている場合; それ以外の場合は false .

### isTables() {#isTables--}
```
public boolean isTables()
```


テーブル抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テーブル抽出がサポートされている場合; それ以外の場合は false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


注釈抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if アノテーション抽出がサポートされている場合; それ以外の場合は false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


テンプレートによる解析がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テンプレートによる解析がサポートされている場合; それ以外の場合は false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


フォーム解析がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if フォーム解析がサポートされている場合; それ以外の場合は false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


プレビュー生成がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if プレビュー生成がサポートされている場合; それ以外の場合は false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


ページプレビュー生成がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if ページプレビュー生成がサポートされている場合; それ以外の場合は false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


OCR 機能がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean - OCR機能がサポートされている場合は true、そうでない場合は false。

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


ワークシート抽出がサポートされているかどうかを示す値を取得します。


**Returns:**
boolean - ワークシート抽出がサポートされている場合は true、そうでない場合は false。

