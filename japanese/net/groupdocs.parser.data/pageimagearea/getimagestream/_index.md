---
title: "GetImageStream"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "画像ストリームを返します。"
type: docs
weight: 40
url: /ja/net/groupdocs.parser.data/pageimagearea/getimagestream/
---

## GetImageStream() {#getimagestream}

画像ストリームを返します。

```csharp
public Stream GetImageStream()
```

### 戻り値

画像を含むストリームです。

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
        // 画像ストリームを開く
        using (Stream imageStream = image.GetImageStream())
        {
            // 画像を保存するファイルを作成する
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // 画像ストリームからデータを読み取る
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // ファイルストリームにデータを書き込む
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### 関連項目

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

別の形式で画像ストリームを返します。

```csharp
public Stream GetImageStream(ImageOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | ImageOptions | 画像を抽出するために使用されるオプション。 |

### 戻り値

画像を含むストリームです。

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
        // 画像ストリームを開く
        using (Stream imageStream = image.GetImageStream(options))
        {
            // 画像を保存するファイルを作成する
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // 画像ストリームからデータを読み取る
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // ファイルストリームにデータを書き込む
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### 関連項目

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
