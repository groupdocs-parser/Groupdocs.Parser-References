---
title: "FromExtension"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ファイル拡張子をファイルタイプにマッピングします。"
type: docs
weight: 930
url: /ja/net/groupdocs.parser.options/filetype/fromextension/
---

## FileType.FromExtension method

ファイル拡張子をファイルタイプにマッピングします。

```csharp
public static FileType FromExtension(string extension)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| extension | 文字列 | ファイル拡張子（ピリオド「."」を含む）。 |

### 戻り値

ファイルタイプがサポートされている場合はそれを返し、そうでない場合はデフォルトの [`Unknown`](../unknown) ファイルタイプを返します。

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *extension* が null または空文字列の場合にスローされます。 |

### 関連項目

* class [FileType](../../filetype)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
