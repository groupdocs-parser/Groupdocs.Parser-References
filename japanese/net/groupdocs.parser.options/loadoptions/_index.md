---
title: "LoadOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ファイルを開くために使用されるオプションを提供します。"
type: docs
weight: 420
url: /ja/net/groupdocs.parser.options/loadoptions/
---

## LoadOptions class

ファイルを開くために使用されるオプションを提供します。

```csharp
public sealed class LoadOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | 空の [`Password`](./password) と、[`FileFormat`](./fileformat) が Unknown に等しい新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを、デフォルトのエンコーディングで初期化します。 |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | 空の [`Password`](./password) とデフォルトのエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_5)(FileType) | 空の [`Password`](./password) とデフォルトのエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_9)(string) | [`FileFormat`](./fileformat) が Unknown に等しいデフォルトのエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_10)(TimeSpan) | *timeout* を使用して、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | パスワードとデフォルトのエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_6)(FileType, string) | パスワードとデフォルトのエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | カスタムエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_7)(FileType, string, Encoding, Encoding) | カスタムエンコーディングで、新しい [`LoadOptions`](../loadoptions) クラスのインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_4)(FileFormat, string, Encoding, Encoding, TimeSpan) | 完全にカスタマイズされた [`LoadOptions`](../loadoptions) クラスの新しいインスタンスを初期化します。 |
| [LoadOptions](loadoptions#constructor_8)(FileType, string, Encoding, Encoding, TimeSpan) | 完全にカスタマイズされた [`LoadOptions`](../loadoptions) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | エンコーディング検出に使用されるデフォルトの ANSI エンコーディングを取得します。 |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | ドキュメントのエンコーディングを取得します。 |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | ファイル形式を取得します。 |
| [FileType](../../groupdocs.parser.options/loadoptions/filetype) { get; } | ファイルタイプを取得します。 |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | パスワードを取得します。 |
| [Timeout](../../groupdocs.parser.options/loadoptions/timeout) { get; } | 待機時間（ミリ秒）を表す値を取得します。 |

### 備考

このクラスのインスタンスは、[`Parser`](../../groupdocs.parser/parser) クラスのコンストラクタのパラメータとして使用されます:

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

そこにある使用例をご覧ください。

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
