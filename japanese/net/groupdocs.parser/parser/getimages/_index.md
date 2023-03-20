---
title: GetImages
second_title: GroupDocs.Parser for .NET API リファレンス
description: ドキュメントから画像を抽出します
type: docs
weight: 110
url: /ja/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

ドキュメントから画像を抽出します。

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### 戻り値

のコレクション[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)オブジェクト; `ヌル`画像抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [画像をファイルに抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Microsoft Office Word ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel スプレッドシートから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint プレゼンテーションから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [メールから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例

次の例は、ドキュメント全体からすべての画像を抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // 画像を抽出
    IEnumerable<PageImageArea> images = parser.GetImages();
    // 画像抽出がサポートされているかどうかを確認します
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // 画像を繰り返す
    foreach (PageImageArea image in images)
    {
        // ページ インデックス、四角形、および画像タイプを出力します。
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

カスタマイズ オプション を使用してドキュメントから画像を抽出します (画像を含む四角形の領域を設定します)。

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| options | PageAreaOptions | 画像抽出のオプション。 |

### 戻り値

のコレクション[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)オブジェクト; `ヌル`画像抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [画像をファイルに抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [文書ページ領域から画像を抽出](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel スプレッドシートから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint プレゼンテーションから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [メールから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例

次の例は、左上隅から画像のみを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // 画像抽出に使用するオプションを作成します
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // ページの左上隅から画像を抽出:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // 画像抽出がサポートされているかどうかを確認します
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // 画像を繰り返す
    foreach (PageImageArea image in images)
    {
        // ページ インデックス、四角形、および画像タイプを出力します。
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

ドキュメント ページから画像を抽出します。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |

### 戻り値

のコレクション[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)オブジェクト; `ヌル`画像抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [画像をファイルに抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [ドキュメントページから画像を抽出](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Microsoft Office Word ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel スプレッドシートから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint プレゼンテーションから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [メールから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例

ドキュメント ページから画像を抽出するには、次の方法を使用します。

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントが画像抽出をサポートしているかどうかを確認します
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 画像を繰り返す
        // 以前に画像抽出機能のサポートを確認したため、null チェックは無視します
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // 長方形と画像タイプを出力します
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

カスタマイズ オプション を使用してドキュメント ページから画像を抽出します (画像を含む四角形の領域を設定します)。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |
| options | PageAreaOptions | 画像抽出のオプション。 |

### 戻り値

のコレクション[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)オブジェクト; `ヌル`画像抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [画像をファイルに抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [ドキュメントページから画像を抽出](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [文書ページ領域から画像を抽出](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel スプレッドシートから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint プレゼンテーションから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [メールから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF ドキュメントから画像を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
