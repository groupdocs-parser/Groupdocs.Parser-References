---
title: "パーサー"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テキスト画像コンテナの抽出と解析機能を制御するメインクラスを表します。"
type: docs
weight: 30
url: /ja/net/groupdocs.parser/parser/
---

## Parser class

テキスト、画像、コンテナの抽出および解析機能を制御するメインクラスを表します。

```csharp
public sealed class Parser : IDisposable
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | データベースからデータを抽出するための [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor)(EmailConnection) | リモートメールサーバーからデータを抽出するための [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_4)(Stream) | [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_8)(string) | [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_12)(Uri) | URI からデータを抽出するための [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | データベースからデータを抽出するための [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | リモートメールサーバーからデータを抽出するための [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | [`Parser`](../parser) クラスを [`LoadOptions`](../../groupdocs.parser.options/loadoptions) とともに新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | [`Parser`](../parser) クラスを [`ParserSettings`](../../groupdocs.parser.options/parsersettings) とともに新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_9)(string, LoadOptions) | [`Parser`](../parser) クラスを [`LoadOptions`](../../groupdocs.parser.options/loadoptions) とともに新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_11)(string, ParserSettings) | [`Parser`](../parser) クラスを [`ParserSettings`](../../groupdocs.parser.options/parsersettings) とともに新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | URI からデータを抽出する際に *loadOptions* を使用して [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | URI からデータを抽出する際に *parserSettings* を使用して [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | [`Parser`](../parser) クラスを [`LoadOptions`](../../groupdocs.parser.options/loadoptions) と [`ParserSettings`](../../groupdocs.parser.options/parsersettings) とともに新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | [`Parser`](../parser) クラスを [`LoadOptions`](../../groupdocs.parser.options/loadoptions) と [`ParserSettings`](../../groupdocs.parser.options/parsersettings) とともに新しいインスタンスを初期化します。 |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | URI からデータを抽出する際に *loadOptions* と *parserSettings* を使用して [`Parser`](../parser) クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | サポートされている機能を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | アンマネージドリソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | テンプレートの位置とスケールを自動調整するためのフィールドを生成します。 |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | ページのプレビューを取得します。 |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | ドキュメントから注釈を抽出します。現在、PDF 形式のみがサポートされていることに注意してください。 |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | ドキュメントページから注釈を抽出します。現在、PDF 形式のみがサポートされていることに注意してください。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | ドキュメントからバーコードを抽出します。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | カスタマイズオプションを使用して、ドキュメントからバーコードを抽出します。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | ドキュメントページからバーコードを抽出します。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | カスタマイズオプションを使用して、ドキュメントページからバーコードを抽出します。 |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | 添付ファイルやZIPアーカイブなどを含む形式を扱うために、ドキュメントからコンテナオブジェクトを抽出します。 |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | ドキュメントに関する一般情報を返します。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | ドキュメントから書式付きテキストを抽出します。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | ドキュメントページから書式付きテキストを抽出します。 |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | ドキュメントからハイライトを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | ドキュメントからハイパーリンクを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | ドキュメントページからハイパーリンクを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | ハイパーリンクを含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントからハイパーリンクを抽出します。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | ハイパーリンクを含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントページからハイパーリンクを抽出します。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | ドキュメントから画像を抽出します。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | ドキュメントページから画像を抽出します。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | 画像を含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントから画像を抽出します。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | 画像を含む矩形領域を設定するカスタマイズオプションを使用して、ドキュメントページから画像を抽出します。 |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | ドキュメントからメタデータを抽出します。 |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | ドキュメントページのプレビューを生成します。 |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | カスタマイズオプションを使用して、ドキュメントページのプレビューを生成します。 |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | ドキュメントから構造化テキストを抽出します。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | ドキュメントからテーブルを抽出します。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | ドキュメントページからテーブルを抽出します。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | ドキュメントからテーブルを抽出します。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | ドキュメントページからテーブルを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | ドキュメントからテキストを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | ドキュメントページからテキストを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | 生の高速テキスト抽出モードを有効にするテキストオプションを使用して、ドキュメントからテキストページを抽出します。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | テキストオプションを使用してドキュメントページからテキストを抽出します（生の高速テキスト抽出モードを有効にするため）。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | ドキュメントからテキスト領域を抽出します。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | ドキュメントページからテキスト領域を抽出します。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | カスタマイズオプション（正規表現、大小文字の一致など）を使用してドキュメントからテキスト領域を抽出します。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | カスタマイズオプション（正規表現、大小文字の一致など）を使用してドキュメントページからテキスト領域を抽出します。 |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | ドキュメントから目次を抽出します。 |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | ワークシートのセルを抽出します。 |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | カスタマイズオプションを使用してワークシートのセルを抽出します。 |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | スプレッドシート内のすべてのワークシートに関する情報を抽出します。 |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | ワークシートに関する情報を抽出します。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | ユーザー作成テンプレートでドキュメントを解析します。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | カスタマイズオプションを使用してユーザー作成テンプレートでドキュメントを解析します。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | 提供されたコレクションから最適なテンプレートを選択し、選択したテンプレートに対してドキュメントを解析します。 |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | ドキュメントフォームを解析します。 |
| [Search](../../groupdocs.parser/parser/search#search)(string) | ドキュメント内で*keyword*を検索します。 |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | 検索オプション（正規表現、大小文字の一致など）を使用してドキュメント内で*keyword*を検索します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | ファイルに関する一般情報を返します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | ファイルに関する一般情報を返します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | ファイルに関する一般情報を返します。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | ファイルに関する一般情報を返します。 |

### 関連項目

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
