---
title: "ContainerItem"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "Zip アーカイブエンティティ、メール添付ファイル、PDF ポートフォリオ アイテムなどのコンテナ アイテムを表します。"
type: docs
weight: 720
url: /ja/net/groupdocs.parser.data/containeritem/
---

## ContainerItem class

Zip アーカイブエンティティ、メール添付、PDF ポートフォリオ項目などのコンテナ項目を表します。

```csharp
public sealed class ContainerItem
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | アイテムのディレクトリを取得します。 |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | アイテムのフルパスを取得します。 |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | メタデータ アイテムのコレクションを取得します。 |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | アイテムの名前を取得します。 |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | アイテムのサイズを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | コンテナ アイテムのファイルタイプを検出します。 |
| [GetMetadataValue](../../groupdocs.parser.data/containeritem/getmetadatavalue)(string) | メタデータの値を取得します。 |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | アイテム コンテンツ用に [`Parser`](../../groupdocs.parser/parser) オブジェクトを作成します。 |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | アイテム コンテンツ用に [`LoadOptions`](../../groupdocs.parser.options/loadoptions) を使用して [`Parser`](../../groupdocs.parser/parser) オブジェクトを作成します。 |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | アイテム コンテンツ用に [`LoadOptions`](../../groupdocs.parser.options/loadoptions) と [`ParserSettings`](../../groupdocs.parser.options/parsersettings) を使用して [`Parser`](../../groupdocs.parser/parser) オブジェクトを作成します。 |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | アイテム コンテンツのストリームを開きます。 |

### 備考

[`ContainerItem`](../containeritem) クラスのインスタンスは [`GetContainer`](../../groupdocs.parser/parser/getcontainer) メソッドの戻り値として使用されます。使用例をご覧ください。

### 関連項目

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
