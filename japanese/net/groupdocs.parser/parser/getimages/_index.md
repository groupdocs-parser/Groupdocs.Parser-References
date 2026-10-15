---
title: "GetImages"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントから画像を抽出します。"
type: docs
weight: 130
url: /ja/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

ドキュメントから画像を抽出します。

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### 戻り値

画像抽出がサポートされていない場合は `null` になる、[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例

以下の例は、ドキュメント全体からすべての画像を抽出する方法を示しています：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // 画像を抽出する
    IEnumerable<PageImageArea> images = parser.GetImages();
    // 画像抽出がサポートされているか確認する
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // 画像を反復処理する
    foreach (PageImageArea image in images)
    {
        // ページインデックス、矩形、画像タイプを出力する：
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

画像を含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントから画像を抽出します。

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | PageAreaOptions | 画像抽出のオプションです。 |

### 戻り値

画像抽出がサポートされていない場合は `null` になる、[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例

以下の例は、左上隅からのみ画像を抽出する方法を示しています：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // 画像抽出に使用されるオプションを作成する
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // ページの左上隅から画像を抽出する：
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // 画像抽出がサポートされているか確認する
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // 画像を反復処理する
    foreach (PageImageArea image in images)
    {
        // ページインデックス、矩形、画像タイプを出力する：
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

ドキュメントページから画像を抽出します。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

画像抽出がサポートされていない場合は `null` になる、[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例

ドキュメントページから画像を抽出するには、以下のメソッドを使用します：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントが画像抽出をサポートしているか確認する
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 画像を反復処理する
        // 以前に画像抽出機能のサポートを確認したので、null チェックは無視します
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // 矩形と画像タイプを出力する
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

画像を含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントページから画像を抽出します。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | PageAreaOptions | 画像抽出のオプションです。 |

### 戻り値

画像抽出がサポートされていない場合は `null` になる、[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 関連項目

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
