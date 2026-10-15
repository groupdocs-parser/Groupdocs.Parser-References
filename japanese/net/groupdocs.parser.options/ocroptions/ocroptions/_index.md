---
title: "OcrOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "矩形領域を使用して OcrOptionsgroupdocs.parser.options/ocroptions クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

矩形領域を使用して、[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions()
```

### 関連項目

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

矩形領域を使用して、[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) クラスのインスタンスで、ドキュメントページプレビュー生成のプロパティを設定します。 |

### 関連項目

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

矩形領域を使用して、[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions(Rectangle rectangle)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| rectangle | 矩形 | テキスト認識に使用されるページ領域を制約する矩形領域です。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

[`OcrEventHandler`](../../ocreventhandler) オブジェクトを使用して、[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions(OcrEventHandler handler)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| handler | OcrEventHandler | OCR イベントを捕捉するための [`OcrEventHandler`](../../ocreventhandler) のインスタンスです。 |

### 関連項目

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

矩形領域と [`OcrEventHandler`](../../ocreventhandler) オブジェクトを使用して、[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| rectangle | 矩形 | テキスト認識に使用されるページ領域を制約する矩形領域です。 |
| handler | OcrEventHandler | OCR イベントを捕捉するための [`OcrEventHandler`](../../ocreventhandler) のインスタンスです。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| rectangle | 矩形 | テキスト認識に使用されるページ領域を制約する矩形領域です。 |
| handler | OcrEventHandler | OCR イベントを捕捉するための [`OcrEventHandler`](../../ocreventhandler) のインスタンスです。 |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) クラスのインスタンスで、ドキュメントページプレビュー生成のプロパティを設定します。 |
| useSpellCheker | Boolean | スペルチェッカーが使用されているかどうかを示す値です。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

[`OcrOptions`](../../ocroptions) クラスの新しいインスタンスを初期化します。

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| rectangle | 矩形 | テキスト認識に使用されるページ領域を制約する矩形領域です。 |
| handler | OcrEventHandler | OCR イベントを捕捉するための [`OcrEventHandler`](../../ocreventhandler) のインスタンスです。 |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) クラスのインスタンスで、ドキュメントページプレビュー生成のプロパティを設定します。 |
| useSpellCheker | Boolean | スペルチェッカーが使用されているかどうかを示す値です。 |
| 言語 | 言語 | OCR に使用される言語です。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
