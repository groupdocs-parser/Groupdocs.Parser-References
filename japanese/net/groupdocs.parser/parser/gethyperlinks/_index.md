---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからハイパーリンクを抽出します。"
type: docs
weight: 120
url: /ja/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

ドキュメントからハイパーリンクを抽出します。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### 戻り値

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション。ハイパーリンク抽出がサポートされていない場合は `null`。

### 例

次の例は、ドキュメント全体からすべてのハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているか確認する
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // ドキュメントからハイパーリンクを抽出する
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // ハイパーリンクを反復処理する
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // ハイパーリンクのテキストを出力する
        Console.WriteLine(h.Text);
        // ハイパーリンクの URL を出力する
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

ドキュメントページからハイパーリンクを抽出します。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション。ハイパーリンク抽出がサポートされていない場合は `null`。

### 例

次の例は、ドキュメントページからハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているか確認する
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // ページを反復処理する
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // ドキュメントページからハイパーリンクを抽出する
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // ハイパーリンクを反復処理する
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // ハイパーリンクのテキストを出力する
            Console.WriteLine(h.Text);
            // ハイパーリンクの URL を出力する
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

ハイパーリンクを含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントからハイパーリンクを抽出します。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | PageAreaOptions | ハイパーリンク抽出のオプション。 |

### 戻り値

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション。ハイパーリンク抽出がサポートされていない場合は `null`。

### 例

次の例は、ドキュメントページ領域からハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているか確認する
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // ハイパーリンク抽出に使用されるオプションを作成する
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // ドキュメントページ領域からハイパーリンクを抽出する
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // ハイパーリンクを反復処理する
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // ハイパーリンクのテキストを出力する
        Console.WriteLine(h.Text);
        // ハイパーリンクの URL を出力する
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

ハイパーリンクを含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントページからハイパーリンクを抽出します。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | PageAreaOptions | ハイパーリンク抽出のオプション。 |

### 戻り値

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) オブジェクトのコレクション。ハイパーリンク抽出がサポートされていない場合は `null`。

### 例

次の例は、カスタマイズオプションを使用してドキュメントページ領域からハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているか確認する
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // ハイパーリンク抽出に使用されるオプションを作成する
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // ページを反復処理する
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // ドキュメントページ領域からハイパーリンクを抽出する
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // ハイパーリンクを反復処理する
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // ハイパーリンクのテキストを出力する
            Console.WriteLine(h.Text);
            // ハイパーリンクの URL を出力する
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
