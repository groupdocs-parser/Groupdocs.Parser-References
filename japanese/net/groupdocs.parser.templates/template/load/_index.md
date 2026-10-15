---
title: "Load"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ファイルからテンプレートを読み込みます。"
type: docs
weight: 20
url: /ja/net/groupdocs.parser.templates/template/load/
---

## Load(string) {#load_1}

ファイルからテンプレートを読み込みます。

```csharp
public static Template Load(string filePath)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |

### 戻り値

ロードされたテンプレートを持つ [`Template`](../../template) クラスのインスタンスです。

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | ファイルは有効な形式のテンプレートを表していません。 |

### 関連項目

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Load(Stream) {#load}

ストリームからテンプレートを読み込みます。

```csharp
public static Template Load(Stream stream)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ストリーム | Stream | 入力ストリームです。 |

### 戻り値

ロードされたテンプレートを持つ [`Template`](../../template) クラスのインスタンスです。

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | ストリームは有効な形式のテンプレートを表していません。 |

### 関連項目

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
