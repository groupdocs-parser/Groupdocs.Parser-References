---
title: GetHyperlinks
second_title: GroupDocs.Parser for .NET API リファレンス
description: ドキュメントからハイパーリンクを抽出します
type: docs
weight: 100
url: /ja/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

ドキュメントからハイパーリンクを抽出します。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### 戻り値

のコレクション[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)オブジェクト; `ヌル`ハイパーリンク抽出がサポートされていない場合.

### 例

次の例は、ドキュメント全体からすべてのハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているかどうかを確認します
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // ドキュメントからハイパーリンクを抽出します
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // ハイパーリンクを繰り返す
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // ハイパーリンク テキストを出力します
        Console.WriteLine(h.Text);
        // ハイパーリンクの URL を出力
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

ドキュメント ページからハイパーリンクを抽出します。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |

### 戻り値

のコレクション[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)オブジェクト; `ヌル`ハイパーリンク抽出がサポートされていない場合.

### 例

次の例は、ドキュメント ページからハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているかどうかを確認します
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるかどうかを確認します
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // ページを繰り返す
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // ドキュメント ページからハイパーリンクを抽出します
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // ハイパーリンクを繰り返す
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // ハイパーリンク テキストを出力します
            Console.WriteLine(h.Text);
            // ハイパーリンクの URL を出力
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

カスタマイズ オプション を使用してドキュメントからハイパーリンクを抽出します (ハイパーリンクを含む四角形の領域を設定します)。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| options | PageAreaOptions | ハイパーリンク抽出のオプション。 |

### 戻り値

のコレクション[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)オブジェクト; `ヌル`ハイパーリンク抽出がサポートされていない場合.

### 例

次の例は、ドキュメント ページ領域からハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているかどうかを確認します
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // ハイパーリンク抽出に使用されるオプションを作成します
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // ドキュメント ページ領域からハイパーリンクを抽出します
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // ハイパーリンクを繰り返す
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // ハイパーリンク テキストを出力します
        Console.WriteLine(h.Text);
        // ハイパーリンクの URL を出力
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

カスタマイズ オプション を使用してドキュメント ページからハイパーリンクを抽出します (ハイパーリンクを含む四角形の領域を設定します)。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |
| options | PageAreaOptions | ハイパーリンク抽出のオプション。 |

### 戻り値

のコレクション[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)オブジェクト; `ヌル`ハイパーリンク抽出がサポートされていない場合.

### 例

次の例は、カスタマイズ オプションを使用してドキュメント ページ領域からハイパーリンクを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがハイパーリンク抽出をサポートしているかどうかを確認します
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるかどうかを確認します
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // ハイパーリンク抽出に使用されるオプションを作成します
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // ページを繰り返す
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // ドキュメント ページ領域からハイパーリンクを抽出します
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // ハイパーリンクを繰り返す
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // ハイパーリンク テキストを出力します
            Console.WriteLine(h.Text);
            // ハイパーリンクの URL を出力
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### 関連項目

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
