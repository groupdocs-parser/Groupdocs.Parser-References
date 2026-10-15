---
title: "保存"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "画像をファイルに保存します。"
type: docs
weight: 50
url: /ja/net/groupdocs.parser.data/pageimagearea/save/
---

## Save(string) {#save}

画像をファイルに保存します。

```csharp
public void Save(string filePath)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |

### 例

次の例は画像をファイルに保存する方法を示しています：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントから画像を抽出する
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // 画像抽出がサポートされているか確認する
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // 画像を反復処理する
    foreach (PageImageArea image in images)
    {
        // 画像をファイルに保存します。
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### 関連項目

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

画像を別の形式でファイルに保存します。

```csharp
public void Save(string filePath, ImageOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |
| options | ImageOptions | 画像を保存するために使用されるオプション。 |

### 例

次の例は、画像を別の形式でファイルに保存する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントから画像を抽出する
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // 画像抽出がサポートされているか確認する
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // PNG 形式で画像を保存するためのオプションを作成します。
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // 画像を反復処理する
    foreach (PageImageArea image in images)
    {
        // 画像を PNG ファイルに保存します。
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### 関連項目

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
