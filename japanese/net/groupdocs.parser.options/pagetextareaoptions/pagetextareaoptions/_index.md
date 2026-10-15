---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "OCR 使用オプションを指定して PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

OCR 使用オプションを指定して [`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。

```csharp
public PageTextAreaOptions()
```

### 関連項目

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

OCR 使用オプションを指定して [`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| useOcr | Boolean | テキスト領域を抽出するために OCR 機能が使用されているかどうかを示す値です。 |

### 関連項目

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

OCR オプションを設定できるように [`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| useOcr | Boolean | テキスト領域を抽出するために OCR 機能が使用されているかどうかを示す値です。 |
| ocrOptions | OcrOptions | OCR 機能の追加オプションです。 |

### 関連項目

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

正規表現を指定して [`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。その他のオプションはデフォルトで設定されます（詳細は備考を参照）。

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| expression | 文字列 | 正規表現です。 |

### 備考

以下のプロパティはデフォルト値を持ちます：

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### 関連項目

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

正規表現と矩形領域を指定して [`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。その他のオプションはデフォルトで設定されます（詳細は備考を参照）。

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| expression | 文字列 | 正規表現です。 |
| rectangle | 矩形 | ページ領域を含む矩形領域です。 |

### 備考

以下のプロパティはデフォルト値を持ちます：

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

正規表現、矩形領域、および無視される境界のサイズを指定して [`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。その他のオプションはデフォルトで設定されます（詳細は備考を参照）。

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| expression | 文字列 | 正規表現です。 |
| rectangle | 矩形 | ページ領域を含む矩形領域です。 |
| rectangleTolerance | Double | 矩形領域で取得される際に無視される境界のサイズです。テキスト項目の高さの割合で測定されます。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

[`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを初期化します。

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| expression | 文字列 | 正規表現です。 |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| uniteSegments | Boolean | セグメントが結合されているかどうかを示す値。 |
| ignoreFormatting | Boolean | テキストの書式設定が無視されるかどうかを示す値。 |
| rectangle | 矩形 | ページ領域を含む矩形領域です。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

[`PageTextAreaOptions`](../../pagetextareaoptions) クラスの新しいインスタンスを、無視される境界のサイズと共に初期化します。

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| expression | 文字列 | 正規表現です。 |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| uniteSegments | Boolean | セグメントが結合されているかどうかを示す値。 |
| ignoreFormatting | Boolean | テキストの書式設定が無視されるかどうかを示す値。 |
| rectangle | 矩形 | ページ領域を含む矩形領域です。 |
| rectangleTolerance | Double | 矩形領域で取得される際に無視される境界のサイズです。テキスト項目の高さの割合で測定されます。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
