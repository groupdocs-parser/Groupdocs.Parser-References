---
title: "SearchOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "SearchOptionsgroupdocs.parser.options/searchoptions クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

[`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| matchWholeWord | Boolean | テキスト検索が単語全体で制限されるかどうかを示す値です。 |
| useRegularExpression | Boolean | 正規表現が使用されているかどうかを示す値です。 |
| searchByPages | Boolean | 検索がページ単位で実行されるかどうかを示す値です。 |
| leftHighlightOptions | HighlightOptions | 左側ハイライトのオプションです。 |
| rightHighlightOptions | HighlightOptions | 右側ハイライトのオプションです。 |

### 関連項目

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

ページ制限付きで [`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| matchWholeWord | Boolean | テキスト検索が単語全体で制限されるかどうかを示す値です。 |
| useRegularExpression | Boolean | 正規表現が使用されているかどうかを示す値です。 |
| maxPageIndex | Int32 | 検索がページ単位で実行されるかどうかを示す値です。 |
| leftHighlightOptions | HighlightOptions | 左側ハイライトのオプションです。 |
| rightHighlightOptions | HighlightOptions | 右側ハイライトのオプションです。 |

### 関連項目

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

左と右のハイライト抽出のためのハイライトオプションを使用して検索するための、[`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| matchWholeWord | Boolean | テキスト検索が単語全体で制限されるかどうかを示す値です。 |
| useRegularExpression | Boolean | 正規表現が使用されているかどうかを示す値です。 |
| leftHighlightOptions | HighlightOptions | 左側ハイライトのオプションです。 |
| rightHighlightOptions | HighlightOptions | 右側ハイライトのオプションです。 |

### 関連項目

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

左側と右側のハイライト抽出に同じハイライトオプションを使用して検索するための、[`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| matchWholeWord | Boolean | テキスト検索が単語全体で制限されるかどうかを示す値です。 |
| useRegularExpression | Boolean | 正規表現が使用されているかどうかを示す値です。 |
| highlightOptions | HighlightOptions | 両方のハイライトのオプションです。 |

### 関連項目

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

ハイライト抽出なしで検索するための、[`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| matchWholeWord | Boolean | テキスト検索が単語全体で制限されるかどうかを示す値です。 |
| useRegularExpression | Boolean | 正規表現が使用されているかどうかを示す値です。 |

### 関連項目

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

ページ単位で検索し、ハイライト抽出なしで検索するための、[`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| matchCase | Boolean | テキストの大文字小文字が無視されないかどうかを示す値。 |
| matchWholeWord | Boolean | テキスト検索が単語全体で制限されるかどうかを示す値です。 |
| useRegularExpression | Boolean | 正規表現が使用されているかどうかを示す値です。 |
| searchByPages | Boolean | 検索がページ単位で実行されるかどうかを示す値です。 |

### 関連項目

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

デフォルト値で [`SearchOptions`](../../searchoptions) クラスの新しいインスタンスを初期化します。詳細は備考をご覧ください。

```csharp
public SearchOptions()
```

### 備考

以下のプロパティはデフォルト値を持ちます：

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### 関連項目

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
