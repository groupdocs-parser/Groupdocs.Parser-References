---
title: "DetectFileType"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "コンテナ アイテムのファイルタイプを検出します。"
type: docs
weight: 60
url: /ja/net/groupdocs.parser.data/containeritem/detectfiletype/
---

## ContainerItem.DetectFileType method

コンテナ アイテムのファイルタイプを検出します。

```csharp
public FileType DetectFileType(FileTypeDetectionMode detectionMode)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| detectionMode | FileTypeDetectionMode | ファイルタイプ検出のモードを定義します。 |

### 戻り値

[`FileType`](../../../groupdocs.parser.options/filetype) クラスのインスタンス；ファイルタイプが検出されない場合は [`Unknown`](../../../groupdocs.parser.options/filetype/unknown) です。

### 備考

*detectionMode* parameter provides the ability to control file type detection:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

### 例

以下の例は、コンテナ項目のファイルタイプを検出する方法を示しています：

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // コンテナから添付ファイルを抽出する
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // コンテナ抽出がサポートされているか確認する
    if (attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
    // 添付ファイルを反復処理する
    foreach (ContainerItem item in attachments)
    {
        // ファイルタイプを検出する
        Options.FileType fileType = item.DetectFileType(Options.FileTypeDetectionMode.Default);

        // 名前とファイルタイプを出力する
        Console.WriteLine(string.Format("{0}: {1}", item.Name, fileType));
    }
}
```

### 関連項目

* class [FileType](../../../groupdocs.parser.options/filetype)
* enum [FileTypeDetectionMode](../../../groupdocs.parser.options/filetypedetectionmode)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
