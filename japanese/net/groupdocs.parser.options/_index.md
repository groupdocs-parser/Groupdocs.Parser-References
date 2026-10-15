---
title: "GroupDocs.Parser.Options"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "この名前空間は、ドキュメントからデータを解析する際の追加オプションを指定するクラスを提供します。"
type: docs
weight: 50
url: /ja/net/groupdocs.parser.options/
---

この名前空間は、ドキュメントからデータを解析する際の追加オプションを指定するクラスを提供します。

## クラス

| クラス | 説明 |
| --- | --- |
| [AdjustmentFieldsOptions](./adjustmentfieldsoptions) | 調整フィールドを生成するために使用されるオプションを提供します。 |
| [BarcodeOptions](./barcodeoptions) | バーコード抽出に使用されるオプションを提供します。 |
| [CreatePageStream](./createpagestream) | ページプレビュー データを書き込むためのストリームを返すメソッドを表します。 |
| [DocumentInfo](./documentinfo) | ドキュメント情報を表します。 |
| [EmailConnection](./emailconnection) | メール接続情報を表します。 |
| [EmailEwsConnection](./emailewsconnection) | EWS プロトコル用のメール接続情報を表します。 |
| [EmailImapConnection](./emailimapconnection) | IMAP プロトコル用のメール接続情報を表します。 |
| [EmailPopConnection](./emailpopconnection) | POP プロトコル用のメール接続情報を表します。 |
| [ExternalResourceHandler](./externalresourcehandler) | 外部リソースの読み込み用ハンドラを提供します。 |
| [ExternalResourceLoadingArgs](./externalresourceloadingargs) | [`OnLoading`](../groupdocs.parser.options/externalresourcehandler/onloading) メソッドのデータを提供します。 |
| [Features](./features) | サポートされている機能の一覧を表します。ドキュメントでサポートされているかどうかの情報を取得できます。 |
| [FileInfo](./fileinfo) | ファイル情報を表します。 |
| [FileType](./filetype) | ファイルタイプを表します。**GroupDocs.Parser** がサポートするすべてのファイルタイプの一覧を取得するメソッドを提供します。 |
| [FormattedTextOptions](./formattedtextoptions) | 書式付きテキスト抽出に使用されるオプションを提供します。 |
| [HighlightOptions](./highlightoptions) | ハイライト（検索シナリオで見つかったテキストの周囲のテキストブロック）を抽出するために使用されるオプションを提供します。 |
| [ImageOptions](./imageoptions) | 画像抽出に使用されるオプションを提供します。 |
| [LoadOptions](./loadoptions) | ファイルを開くために使用されるオプションを提供します。 |
| [OcrConnectorBase](./ocrconnectorbase) | OCR 機能を提供します。 |
| [OcrEventHandler](./ocreventhandler) | OCR イベント用ハンドラを提供します。 |
| [OcrOptions](./ocroptions) | OCR コネクタに使用されるオプションを提供します。 |
| [PageAreaOptions](./pageareaoptions) | ページ領域抽出に使用されるオプションを提供します。 |
| [PageInfo](./pageinfo) | ドキュメントページ情報を表します。 |
| [PagePreviewOptions](./pagepreviewoptions) | ドキュメントページプレビューを生成するために使用されるオプションを提供します。 |
| [PageRenderInfo](./pagerenderinfo) | ページがどのようにレンダリングされるかの情報を表します。 |
| [PageTableAreaOptions](./pagetableareaoptions) | ページテーブル領域の抽出に使用されるオプションを提供します。 |
| [PageTextAreaOptions](./pagetextareaoptions) | ページテキスト領域の抽出に使用されるオプションを提供します。 |
| [ParseByTemplateOptions](./parsebytemplateoptions) | テンプレートによる解析に使用されるオプションを提供します。 |
| [ParserSettings](./parsersettings) | データ抽出をカスタマイズするために使用される設定を提供します。 |
| [PreviewOptions](./previewoptions) | プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。 |
| [PreviewPageRender](./previewpagerender) | ドキュメントページがレンダリングされる前に呼び出されるメソッドを表します。 |
| [ReleasePageStream](./releasepagestream) | [`CreatePageStream`](../groupdocs.parser.options/createpagestream) デリゲートによって作成されたストリームを解放するメソッドを表します。 |
| [SearchOptions](./searchoptions) | テキスト検索に使用されるオプションを提供します。 |
| [TextDocumentInfo](./textdocumentinfo) | テキストドキュメント情報を表します。 |
| [TextOptions](./textoptions) | テキスト抽出に使用されるオプションを提供します。 |
| [WorksheetOptions](./worksheetoptions) | ワークシート抽出に使用されるオプションを提供します。 |
## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [IDocumentInfo](./idocumentinfo) | ドキュメント情報を表します。 |
| [ILogger](./ilogger) | データ抽出中のイベントやエラーのロギングに使用されるロガーのインターフェイスを定義します。 |
## 列挙体

| 列挙体 | 説明 |
| --- | --- |
| [FileFormat](./fileformat) | ファイルのタイプを定義します。 |
| [FileTypeDetectionMode](./filetypedetectionmode) | ファイルタイプ検出のモードを定義します。 |
| [FormattedTextMode](./formattedtextmode) | 書式付きテキストモードを定義します。 |
| [ImageFormat](./imageformat) | 画像のフォーマットを定義します。 |
| [Language](./language) | 光学文字認識（OCR）に使用される言語を定義します。ISO 939-3 コードが使用されます。 |
| [PagePreviewFormat](./pagepreviewformat) | サポートされているプレビュー形式を表します。 |
| [PreviewOptions.PreviewFormats](./previewoptions.previewformats) | サポートされているプレビュー形式を表します。 |
| [QualityMode](./qualitymode) | 品質のレベルを定義します。 |

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
