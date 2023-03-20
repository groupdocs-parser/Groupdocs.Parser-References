---
title: Parser
second_title: GroupDocs.Parser for .NET API リファレンス
description: テキスト画像コンテナ抽出および解析機能を制御するメイン クラスを表します
type: docs
weight: 640
url: /ja/net/groupdocs.parser/parser/
---
## Parser class

テキスト、画像、コンテナ抽出および解析機能を制御するメイン クラスを表します。

```csharp
public sealed class Parser : IDisposable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | の新しいインスタンスを初期化します[`Parser`](../parser)データベースからデータを抽出するクラス. |
| [Parser](parser#constructor)(EmailConnection) | の新しいインスタンスを初期化します[`Parser`](../parser)リモート電子メール サーバーからデータを抽出するクラス. |
| [Parser](parser#constructor_4)(Stream) | の新しいインスタンスを初期化します[`Parser`](../parser)class. |
| [Parser](parser#constructor_8)(string) | の新しいインスタンスを初期化します[`Parser`](../parser)class. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | の新しいインスタンスを初期化します[`Parser`](../parser)データベースからデータを抽出するクラス. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | の新しいインスタンスを初期化します[`Parser`](../parser)リモート電子メール サーバーからデータを抽出するクラス. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | の新しいインスタンスを初期化します[`Parser`](../parser)クラス[`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | の新しいインスタンスを初期化します[`Parser`](../parser)クラス[`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | の新しいインスタンスを初期化します[`Parser`](../parser)クラス[`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | の新しいインスタンスを初期化します[`Parser`](../parser)クラス[`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | の新しいインスタンスを初期化します[`Parser`](../parser)クラス[`LoadOptions`](../../groupdocs.parser.options/loadoptions) と[`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | の新しいインスタンスを初期化します[`Parser`](../parser)クラス[`LoadOptions`](../../groupdocs.parser.options/loadoptions) と[`ParserSettings`](../../groupdocs.parser.options/parsersettings). |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | サポートされている機能を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | アンマネージ リソースの解放、解放、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | ページのプレビューを取得します。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | ドキュメントからバーコードを抽出します。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | ドキュメント ページからバーコードを抽出します。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | カスタマイズ オプション を使用してドキュメントからバーコードを抽出します (バーコードを含む四角形の領域を設定します)。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | カスタマイズ オプション (バーコードを含む長方形の領域を設定するため) を使用して、ドキュメント ページからバーコードを抽出します。 |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | ドキュメントからコンテナー オブジェクトを抽出して、添付ファイル、ZIP アーカイブなどを含む形式を操作します。 |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | ドキュメントに関する一般情報を返します。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | ドキュメントから書式設定されたテキストを抽出します。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | ドキュメント ページから書式設定されたテキストを抽出します。 |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | ドキュメントからハイライトを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | ドキュメントからハイパーリンクを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | ドキュメント ページからハイパーリンクを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | カスタマイズ オプション を使用してドキュメントからハイパーリンクを抽出します (ハイパーリンクを含む四角形の領域を設定します)。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | カスタマイズ オプション を使用してドキュメント ページからハイパーリンクを抽出します (ハイパーリンクを含む四角形の領域を設定します)。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | ドキュメントから画像を抽出します。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | ドキュメント ページから画像を抽出します。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | カスタマイズ オプション を使用してドキュメントから画像を抽出します (画像を含む四角形の領域を設定します)。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | カスタマイズ オプション を使用してドキュメント ページから画像を抽出します (画像を含む四角形の領域を設定します)。 |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | ドキュメントからメタデータを抽出します。 |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | ドキュメントから構造化テキストを抽出します。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | ドキュメントからテーブルを抽出します。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | ドキュメント ページからテーブルを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | ドキュメントからテキストを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | ドキュメント ページからテキストを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | テキスト オプションを使用してドキュメントからテキスト ページを抽出します (生の高速テキスト抽出モードを有効にするため)。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | テキスト オプションを使用してドキュメント ページからテキストを抽出します (生の高速テキスト抽出モードを有効にするため)。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | ドキュメントからテキスト領域を抽出します。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | ドキュメント ページからテキスト領域を抽出します。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | カスタマイズ オプション (正規表現、大文字と小文字の一致など) を使用してドキュメントからテキスト領域を抽出します。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | カスタマイズ オプション (正規表現、大文字と小文字の一致など) を使用してドキュメント ページからテキスト領域を抽出します。 |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | ドキュメントから目次を抽出します。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | ユーザーが生成したテンプレートによってドキュメントを解析します. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | ドキュメント フォームを解析します。 |
| [Search](../../groupdocs.parser/parser/search#search)(string) | 検索します*keyword*ドキュメント内. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | 検索します*keyword*検索オプション (正規表現、大文字と小文字の一致など) を使用してドキュメント内で。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | ファイルに関する一般的な情報を返します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | ファイルに関する一般的な情報を返します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | ファイルに関する一般的な情報を返します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | ファイルに関する一般的な情報を返します。 |

### 関連項目

* 名前空間 [GroupDocs.Parser](../../groupdocs.parser)
* 組み立て [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
