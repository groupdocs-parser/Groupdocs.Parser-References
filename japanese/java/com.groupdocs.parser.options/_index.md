---
title: "com.groupdocs.parser.options"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "このパッケージは、ドキュメントからデータを解析する際に追加オプションを指定するクラスを提供します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.parser.options/
---

このパッケージは、ドキュメントからデータを解析する際に追加オプションを指定するクラスを提供します。



## クラス

| クラス | 説明 |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | バーコード抽出に使用されるオプションを提供します。 |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | ドキュメント情報を表します。 |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | メール接続情報を表します。 |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | EWS プロトコル用のメール接続情報を表します。 |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | IMAP プロトコル用のメール接続情報を表します。 |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | POP プロトコル用のメール接続情報を表します。 |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | 外部リソースの読み込み用ハンドラを提供します。 |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) メソッドのデータを提供します。 |
| [Features](../com.groupdocs.parser.options/features) | サポートされている機能の一覧を表します。 |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | ファイル情報を表します。 |
| [FileType](../com.groupdocs.parser.options/filetype) | ファイルタイプを表します。 |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | 書式付きテキスト抽出に使用されるオプションを提供します。 |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | 検索シナリオで見つかったテキストの周囲のテキストブロック（ハイライト）を抽出するために使用されるオプションを提供します。 |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | 画像抽出に使用されるオプションを提供します。 |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | ファイルを開くために使用されるオプションを提供します。 |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | OCR機能を提供します。 |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | OCRイベント用ハンドラを提供します。 |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | OCRコネクタに使用されるオプションを提供します。 |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | ページ領域抽出に使用されるオプションを提供します。 |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | ドキュメントページ情報を表します。 |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | ページがどのようにレンダリングされるかの情報を表します。 |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | ページテーブル領域抽出に使用されるオプションを提供します。 |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | ページテキスト領域抽出に使用されるオプションを提供します。 |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用される設定を提供します。 |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。 |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | テキスト検索に使用されるオプションを提供します。 |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | テキストドキュメント情報を表します。 |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | テキスト抽出に使用されるオプションを提供します。 |

## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | ページプレビュー データを書き込むためのストリームを返すデリゲートを表します。 |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | ドキュメント情報を表します。 |
| [ILogger](../com.groupdocs.parser.options/ilogger) | データ抽出中のイベントやエラーの記録に使用されるロガーのインターフェイスを定義します。 |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | ドキュメントページがレンダリングされる前に呼び出されるメソッドを表します。 |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) デリゲートによって作成されたストリームを解放するメソッドを表します。 |

## 列挙型

| 列挙体 | 説明 |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | ファイルのタイプを定義します。 |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | ファイルタイプ検出のモードを定義します。 |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | 書式化テキストモードを定義します。 |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | 画像のフォーマットを定義します。 |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | サポートされているプレビュー形式を表します。 |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | 品質のレベルを定義します。 |
