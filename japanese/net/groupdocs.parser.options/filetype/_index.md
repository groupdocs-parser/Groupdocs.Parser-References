---
title: FileType
second_title: GroupDocs.Parser for .NET API リファレンス
description: ファイルの種類を表しますでサポートされているすべてのファイル タイプのリストを取得するメソッドを提供しますGroupDocs.Parser.
type: docs
weight: 380
url: /ja/net/groupdocs.parser.options/filetype/
---
## FileType class

ファイルの種類を表します。でサポートされているすべてのファイル タイプのリストを取得するメソッドを提供します。**GroupDocs.Parser**.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | ファイル名のサフィックス (ピリオド "." を含む) 例: ".doc". |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | ファイルの種類名 (例: "Microsoft Word ドキュメント". |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | ファイルのフォーマット、例えば「WordProcessing」. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | ファイル拡張子をファイル タイプにマップします。 |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 現在の[`FileType`](../filetype)指定と同じです[`FileType`](../filetype)object. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 現在の[`FileType`](../filetype)指定されたオブジェクトと同じです. |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 現在のハッシュ コードを返します。[`FileType`](../filetype)object. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 現在のオブジェクトを表す文字列を返します。 |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | サポートされているファイル タイプを取得します |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 2 つの[`FileType`](../filetype)オブジェクトは同じです. |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 2 つの[`FileType`](../filetype)オブジェクトは同じではありません. |

## 田畑

| 名前 | 説明 |
| --- | --- |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | 拡張子が .BMP のファイルは、ビットマップ デジタル イメージを格納するために使用されるビットマップ イメージ ファイルを表します。このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/bmp/). |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | Bzip2 アルゴリズムを使用した圧縮ファイル。 |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile (CGM) は、ベクター グラフィックス (2D)、ラスター グラフィックス、およびテキストを格納および交換するための、無料でプラットフォームに依存しない国際標準の metafile 形式です。 このファイル形式について詳しく知る [ここ](https://wiki.fileformat.com/page-description-language/cgm/). |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM ファイル形式は、HTML ページのコレクションで構成される Microsoft HTML ヘルプ ファイルを表します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/chm/). |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | CSV (カンマ区切り値) 拡張子を持つファイルは、コンマ区切り値を持つデータのレコードを含むプレーン テキスト ファイル を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/spreadsheet/csv/). |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | 拡張子が .DCM のファイルは、MRI、CT スキャン、超音波画像など、 患者の医療情報を保存するデジタル画像を表します。 このファイル形式について詳しく知る [ここ](https://wiki.fileformat.com/image/dcm/). |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB (Device Independent Bitmap) ファイルは、構造が で標準のビットマップ ファイル (BMP) に似ていますが、ヘッダーが異なるラスター イメージ ファイルです。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/dib/). |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu (「déjà vu」と発音) は、スキャンしたドキュメントや 本、特にテキスト、図、画像、写真の組み合わせを含むものを対象としたグラフィック ファイル形式です。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/djvu/). |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | 拡張子が .doc のファイルは、Microsoft Word またはその他のワード プロセッシングによって生成されたドキュメントを表します ドキュメントはバイナリ ファイル形式です。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/doc/). |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM ファイルは、マクロを実行できる Microsoft Word 2007 以降で生成されたドキュメントです。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/word-processing/docm/). |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX は、Microsoft Word ドキュメントのよく知られた形式です。 2007 年に Microsoft Office 2007 の release で導入されたこの新しいドキュメント形式の構造は、単純な binary から XML とバイナリ ファイルの組み合わせに変更されました。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/docx/). |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | 拡張子が .DOT のファイルは、Microsoft Word によって作成されたテンプレート ファイルであり、さらに DOC または DOCX ファイルを生成するための事前に書式設定された設定 を持っています。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/dot/). |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | DOTM 拡張子を持つファイルは、Microsoft Word 2007 以降で作成されたテンプレート ファイルを表します。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/word-processing/dotm/). |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | DOTX 拡張子を持つファイルは、Microsoft Word によって作成されたテンプレート ファイルであり、さらに DOCX ファイルを生成するための事前にフォーマットされた設定 を持っています。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/dotx/). |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | 拡張メタファイル形式 (EMF) は、グラフィック イメージをデバイスに依存せずに保存します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/emf/) |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML ファイル形式は、Outlook およびその他の関連アプリケーションを使用して保存された電子メール メッセージを表します。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/email/eml/). |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX ファイル形式は、Apple によって実装および開発されています。 Apple Mail アプリケーションは、電子メールのエクスポートに EMLX ファイル形式を使用します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/email/emlx/). |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | EPS 拡張子を持つファイルは、基本的に、単一ページの外観を記述するカプセル化された PostScript 言語プログラム を記述します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/page-description-language/eps/). |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | 拡張子が .EPUB のファイルは、 出版社と消費者向けの標準デジタル出版形式を提供する電子書籍ファイル形式です. このファイル形式の詳細 [ここ](https://wiki.fileformat.com/ebook/epub/). |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | 拡張子が FB2 のファイルは、eBook の構造を含む FictionBook 2.0 eBook ファイルです。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/ebook/fb2/). |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF または Graphical Interchange Format は、高度に圧縮された画像の一種です。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/gif/). |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | 拡張子が .gz のファイルは、gzip 圧縮アプリケーションで作成された圧縮ファイルです。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/compression/gz/). |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | 拡張子が HTM のファイルは、Google Chrome、Internet Explorer、Firefox などの Web ブラウザーで表示するための Web ページ を作成するためのハイパーテキスト マークアップ言語を表します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/htm/). |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML (Hyper Text Markup Language) は、ブラウザーで表示するために作成された Web ページの拡張機能です。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/html/). |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | 拡張子が ICO のファイルは、Microsoft Windows でアプリケーションを表すアイコンとして使用される画像ファイル タイプです。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/ico/). |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000 (J2C) は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を使用して設計された JPEG 2000 は、あらゆる品質のロスレス コンテンツを一度にコーディングできます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/image/jp2/). |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000 (J2K) は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を使用して設計された JPEG 2000 は、あらゆる品質のロスレス コンテンツを一度にコーディングできます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/image/jp2/) |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000 (JP2) は画像符号化システムであり、最先端の画像圧縮規格です。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000 (JPC) は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を使用して設計された JPEG 2000 は、あらゆる品質のロスレス コンテンツを一度にコーディングできます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/image/jp2/) |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG は、非可逆圧縮方式を使用して保存される画像形式の一種です。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000 (JPF) は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を使用して設計された JPEG 2000 は、あらゆる品質のロスレス コンテンツを一度にコーディングできます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG は、非可逆圧縮方式を使用して保存される画像形式の一種です。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を使用して設計された JPEG 2000 は、あらゆる品質のロスレス コンテンツを一度にコーディングできます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を使用して設計された JPEG 2000 は、あらゆる品質のロスレス コンテンツを一度にコーディングできます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/image/jp2/). |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | Markdown 言語の方言で作成されたテキスト ファイルは、 .MD または .MARKDOWN ファイル拡張子で保存されます。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/md/). |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | MHT 拡張子を持つファイルは、さまざまなアプリケーションで 作成できる Web ページ アーカイブ形式を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | MHTML 拡張子を持つファイルは、さまざまなアプリケーションで 作成できる Web ページ アーカイブ形式を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG は、電子メール メッセージ、連絡先、 予定、またはその他のタスクを保存するために Microsoft Outlook および Exchange で使用されるファイル形式です。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/email/msg/). |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | .numbers ファイル拡張子を含むファイルは、 Apple iWork Numbers スプレッドシート アプリケーションによって作成されたファイルです。 |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | ODG ファイル形式は、Apache OpenOffice の Draw アプリケーションで 描画要素をベクター画像として保存するために使用されます。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/odg/). |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | ODP 拡張子を持つファイルは、OASISOpen 標準で OpenOffice.org によって使用されるプレゼンテーション ファイル形式を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/odp/). |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | ODS 拡張子を持つファイルは、ユーザーが編集可能な OpenDocument スプレッドシート ドキュメント形式を表します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/spreadsheet/ods/). |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT ファイルは、OpenDocument テキスト ファイル形式に基づくワード プロセッシング アプリケーションで作成されたドキュメントのタイプです。これらは無料の OpenOffice Writer などのワープロ アプリケーションで作成され、 はテキスト、画像、オブジェクト、スタイルなどのコンテンツを保持できます。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/odt/). |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | .ONE 拡張子で表されるファイルは、Microsoft OneNote アプリケーションによって作成されます。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/note-taking/one/). |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST またはオフライン ストレージ ファイルは、Microsoft Outlook を使用して Exchange Server に 登録すると、ローカル マシン上のオフライン モードでユーザーのメールボックス データを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | 拡張子が .OTP のファイルは、アプリケーション によって OASIS OpenDocument 標準形式で作成されたプレゼンテーション テンプレート ファイルを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/otp/). |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS ファイルには、OpenOffice スプレッドシート アプリケーションで使用されるテンプレート ファイルが含まれています。 |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | OTT 拡張子を持つファイルは、 OASIS の OpenDocument 標準形式に準拠したアプリケーションによって生成されたテンプレート ドキュメントを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/word-processing/ott/). |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL は、Hewlett Packard (HP) によって導入されたページ記述言語 である Printer Command Language の略です。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/page-description-language/pcl/). |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | Portable Document Format (PDF) は、1990 年代に Adobe によって作成されたドキュメントの一種です。この ファイル形式の目的は、アプリケーション ソフトウェア、ハードウェア、およびオペレーティング システムに依存しない 形式でドキュメントやその他の参照資料を表現するための標準を導入することでした。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/view/pdf/). |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT ファイル形式は、ビットマップ イメージとベクター イメージの両方に使用できるメタ形式です。 |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG (Portable Network Graphics) は、ロスレス圧縮を使用するラスター イメージ ファイル形式の一種です。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/png/). |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | .POT 拡張子を持つファイルは、PowerPoint 97-2003 バージョンによって が作成された Microsoft PowerPoint テンプレート ファイルを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/pot/). |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | POTM 拡張子を持つファイルは、マクロをサポートする Microsoft PowerPoint テンプレート ファイルです。 POTM ファイル は PowerPoint 2007 以降で作成され、さらにプレゼンテーション ファイルを作成 するために使用できるデフォルト設定が含まれています。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/potm/). |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | 拡張子が .POTX のファイルは、 Microsoft PowerPoint 2007 以降で作成された Microsoft PowerPoint テンプレート プレゼンテーションを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/potx/). |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS、PowerPoint スライド ショー、ファイルは、スライド ショーの目的で Microsoft PowerPoint を使用して作成されます。 PPS ファイルの読み取りと作成は、Microsoft PowerPoint 97-2003 でサポートされています。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/pps/). |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | PPSM 拡張子を持つファイルは、Microsoft PowerPoint 2007 以降で作成されたマクロ有効スライド ショー ファイル形式を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/ppsm/). |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX、Power Point スライド ショー、ファイルは、 スライド ショーの目的で Microsoft PowerPoint 2007 以降を使用して作成されます。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/ppsx/). |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | 拡張子が PPT のファイルは、スライドショーとして表示される 用のスライドのコレクションで構成される PowerPoint ファイルを表します。 Microsoft PowerPoint 97-2003 で使用されるバイナリ ファイル形式を指定します。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/presentation/ppt/). |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | PPTM 拡張子を持つファイルは、 Microsoft PowerPoint 2007 以降のバージョンで作成された、マクロが有効なプレゼンテーション ファイルです。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/pptm/). |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | 拡張子が PPTX のファイルは、一般的な Microsoft PowerPoint アプリケーションで作成されたプレゼンテーション ファイルです。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/presentation/pptx/). |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) は、デスクトップおよび電子出版のビジネスで 使用される汎用ページ記述言語です。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/page-description-language/ps/). |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD (Photoshop ドキュメント) は、グラフィックスの設計と開発に 使用される Adobe Photoshop のネイティブ ファイル形式を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/psd/). |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | 拡張子が .PST のファイルは、さまざまなユーザー情報を格納する Outlook Personal Storage Files (Personal Storage Table とも呼ばれます) を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | 拡張子が .rar のファイルは、情報を圧縮または通常の形式で保存するために作成されたアーカイブ ファイルを表します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/compression/rar/). |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | Microsoft によって導入および文書化されたリッチ テキスト形式 (RTF) は、アプリケーション内で使用する 形式のテキストとグラフィックスをエンコードする方法を表します。この形式は、他の Microsoft 製品とのクロスプラットフォームの document 交換を容易にし、相互運用性の目的を果たします。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/word-processing/rtf/). |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z は、ファイルやフォルダーを高い圧縮率で圧縮するためのアーカイブ形式です。 このファイル形式について詳しく知る [ここ](https://wiki.fileformat.com/compression/7z/). |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | SVG ファイルは、画像の外観を記述するために XML ベースのテキスト形式 を使用するスカラー ベクター グラフィックス ファイルです。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/page-description-language/svg/). |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | 拡張子が .tar のファイルは、1 つまたは複数のファイルを収集するための Unix ベースのユーティリティで作成されたアーカイブです。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/compression/tar/). |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | 拡張子が .TEXT のファイルは、行形式のプレーン テキストを含むテキスト ドキュメントを表します。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF (Tagged Image File Format) は、このファイル形式標準に準拠するさまざまな デバイスで使用するためのラスター イメージを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF (Tagged Image File Format) は、このファイル形式標準に準拠するさまざまな デバイスで使用するためのラスター イメージを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | Tab-Separated Values (TSV) ファイル形式は、プレーン テキスト形式のタブで区切られたデータを表します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/spreadsheet/tsv/). |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | 拡張子が .TXT のファイルは、行形式のプレーン テキストを含むテキスト ドキュメントを表します。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | 不明なファイル タイプを表します。 |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | Google によって導入された WebP は、可逆圧縮および 非可逆圧縮に基づく最新のラスター Web イメージ ファイル形式です。画像サイズを大幅に縮小しながら、同じ画質を提供します。 このファイル形式の詳細[ここ](https://wiki.fileformat.com/image/webp/). |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | 拡張子が WMF のファイルは、ベクター およびビットマップ形式の画像データを格納するための Microsoft Windows メタファイル (WMF) を表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/image/wmf/) . |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML は、HTML 4.0 の再定式化を使用して、XML にマークアップを含むテキスト ベースのファイル形式です。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/xhtml/). |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | Excel 97-2003 アドイン。追加のコードを実行するように設計された補助プログラムです。 VBA プロジェクトの使用をサポートします。 |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | Excel 2010 および Excel 2007 用の XML ベースでマクロが有効なアドイン形式。 アドインは、追加のコードを実行するように設計された補助プログラムです。 VBA プロジェクトと Excel 4.0 マクロ シート (.xlm) の使用をサポートします。 |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | XLS 拡張子を持つファイルは、Excel Binary File Format を表します。このようなファイルは、Microsoft Excel だけでなく、OpenOffice Calc や Apple Numbers などの他の同様のスプレッドシート プログラムでも作成できます。詳しくは このファイル形式について[ここ](https://wiki.fileformat.com/specification/spreadsheet/xls/). |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB ファイル形式は、Excel ブックのコンテンツを指定するレコードと 構造体のコレクションである Excel バイナリ ファイル形式を指定します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/specification/spreadsheet/xlsb/). |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | 拡張子が XLSM のファイルは、マクロをサポートするスプレッドシート ファイルの一種です。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/specification/spreadsheet/xlsm/). |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX は、Microsoft Office 2007 のリリース で Microsoft によって導入された、Microsoft Excel ドキュメントのよく知られた形式です。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/specification/spreadsheet/xlsx/). |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | 拡張子が .XLT のファイルは、Microsoft Office スイートの一部として提供されるスプレッドシート アプリケーションである Microsoft Excel で作成されたテンプレート ファイルです。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/specification/spreadsheet/xlt/). |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM ファイル拡張子は、マクロが有効な テンプレート ファイルとして Microsoft Excel によって生成されるファイルを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/specification/spreadsheet/xltm/). |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | 拡張子が XLTX のファイルは、Office OpenXML ファイル形式仕様に基づく Microsoft Excel テンプレート ファイルを表します。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/specification/spreadsheet/xltx/). |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML は Extensible Markup Language の略で、HTML に似ていますが、オブジェクトを定義するためのタグの使用が異なります。このファイル形式の詳細 [ここ](https://wiki.fileformat.com/web/xml/). |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP ファイル拡張子は、1 つ以上のファイルまたはディレクトリを保持できるアーカイブを表します。 このファイル形式の詳細 [ここ](https://wiki.fileformat.com/compression/zip/). |

### 備考

**もっと詳しく知る：**

* [サポートされているドキュメント形式](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [サポートされているファイル形式を取得する](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [ドキュメント情報を取得する](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 関連項目

* 名前空間 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 組み立て [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
