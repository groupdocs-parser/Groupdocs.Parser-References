---
title: "FileType"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ファイルタイプを表します。GroupDocs.Parser がサポートするすべてのファイルタイプのリストを取得するメソッドを提供します。"
type: docs
weight: 320
url: /ja/net/groupdocs.parser.options/filetype/
---

## FileType class

ファイルタイプを表します。**GroupDocs.Parser** がサポートするすべてのファイルタイプの一覧を取得するメソッドを提供します。

```csharp
public sealed class FileType : IEquatable<FileType>
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | ファイル名のサフィックス（ピリオド「.」を含む）例: ".doc"。 |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | ファイルタイプ名 例: "Microsoft Word Document"。 |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | ファイルの形式 例: "WordProcessing"。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | ファイル拡張子をファイルタイプにマッピングします。 |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 現在の [`FileType`](../filetype) が指定された [`FileType`](../filetype) オブジェクトと同じかどうかを判断します。 |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 現在の [`FileType`](../filetype) が指定されたオブジェクトと同じかどうかを判断します。 |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 現在の [`FileType`](../filetype) オブジェクトのハッシュコードを返します。 |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 現在のオブジェクトを表す文字列を返します。 |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | サポートされているファイルタイプを取得します |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 2つの [`FileType`](../filetype) オブジェクトが同じかどうかを判断します。 |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 2つの [`FileType`](../filetype) オブジェクトが異なるかどうかを判断します。 |

## Fields

| 名前 | 説明 |
| --- | --- |
| static readonly [AZW3](../../groupdocs.parser.options/filetype/azw3) | AZW3 は Kindle Format 8 (KF8) とも呼ばれ、Amazon Kindle デバイス向けに開発された AZZ 電子書籍デジタルファイル形式の改良版です。このファイル形式の詳細は[here](https://wiki.fileformat.com/ebook/azw3/)でご覧ください。 |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | .BMP 拡張子を持つファイルは、ビットマップ画像ファイルを表し、ビットマップデジタル画像の保存に使用されます。これらの画像はグラフィックアダプタに依存せず、デバイス非依存ビットマップ (DIB) ファイル形式とも呼ばれます。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/bmp/)でご覧ください。 |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | Bzip2 アルゴリズムを使用した圧縮ファイルです。 |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile (CGM) は、ベクターグラフィックス (2D)、ラスタグラフィックス、テキストの保存と交換のための、無料でプラットフォームに依存しない国際標準メタファイル形式です。このファイル形式の詳細は[here](https://wiki.fileformat.com/page-description-language/cgm/)でご覧ください。 |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM ファイル形式は、HTML ページのコレクションで構成される Microsoft HTML ヘルプファイルを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/web/chm/)でご覧ください。 |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | CSV (Comma Separated Values) 拡張子のファイルは、カンマ区切りの値でデータレコードを含むプレーンテキストファイルを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/spreadsheet/csv/)でご覧ください。 |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | .DCM 拡張子のファイルは、MRI、CT スキャン、超音波画像など、患者の医療情報を保存するデジタル画像を表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/dcm/)でご覧ください。 |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB（Device Independent Bitmap）ファイルは、標準のビットマップファイル（BMP）と構造が似ているラスタ画像ファイルですが、ヘッダーが異なります。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/dib/)で確認できます。 |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu（発音は“déjà vu”）は、テキスト、図面、画像、写真が組み合わさったスキャン文書や書籍向けのグラフィックファイル形式です。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/djvu/)で確認できます。 |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | .doc 拡張子のファイルは、Microsoft Word やその他のワードプロセッサで生成されたバイナリ形式の文書を表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/word-processing/doc/)で確認できます。 |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM ファイルは、Microsoft Word 2007 以降で作成され、マクロを実行できる文書です。このファイル形式の詳細は[here](https://wiki.fileformat.com/word-processing/docm/)で確認できます。 |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX は Microsoft Word 文書の代表的な形式です。2007 年に Microsoft Office 2007 がリリースされた際に導入され、従来のバイナリ形式から XML とバイナリファイルの組み合わせに構造が変更されました。このファイル形式の詳細は[here](https://wiki.fileformat.com/word-processing/docx/)で確認できます。 |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | .DOT 拡張子のファイルは、Microsoft Word が作成するテンプレートで、今後生成される DOC または DOCX ファイルのために事前に書式設定された設定を保持します。このファイル形式の詳細は[here](https://wiki.fileformat.com/word-processing/dot/)で確認できます。 |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | DOTM 拡張子のファイルは、Microsoft Word 2007 以降で作成されたテンプレートファイルを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/word-processing/dotm/)で確認できます。 |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | .DOTX 拡張子のファイルは、Microsoft Word が作成するテンプレートで、今後生成される DOCX ファイルのために事前に書式設定された設定を保持します。このファイル形式の詳細は[here](https://wiki.fileformat.com/word-processing/dotx/)で確認できます。 |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | 拡張メタファイル形式（EMF）は、デバイスに依存しない形でグラフィック画像を保存します。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/emf/)で確認できます。 |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML ファイル形式は、Outlook やその他の関連アプリケーションで保存されたメールメッセージを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/email/eml/)で確認できます。 |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX ファイル形式は Apple によって実装・開発されました。Apple Mail アプリケーションはメールのエクスポートに EMLX ファイル形式を使用します。このファイル形式の詳細は[here](https://wiki.fileformat.com/email/emlx/)で確認できます。 |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | .EPS 拡張子のファイルは、基本的に単一ページの外観を記述する Encapsulated PostScript 言語プログラムを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/page-description-language/eps/)で確認できます。 |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | .EPUB 拡張子は、出版社と読者向けに標準的なデジタル出版形式を提供する電子書籍ファイル形式です。このファイル形式の詳細は[here](https://wiki.fileformat.com/ebook/epub/)で確認できます。 |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | .FB2 拡張子のファイルは、eBook の構造を含む FictionBook 2.0 電子書籍ファイルです。このファイル形式の詳細は[here](https://wiki.fileformat.com/ebook/fb2/)で確認できます。 |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF（Graphics Interchange Format）は、高圧縮された画像形式の一種です。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/gif/)で確認できます。 |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | .gz 拡張子のファイルは、gzip 圧縮アプリケーションで作成された圧縮ファイルです。このファイル形式の詳細は[here](https://wiki.fileformat.com/compression/gz/)で確認できます。 |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | .HTM 拡張子のファイルは、Google Chrome、Internet Explorer、Firefox などのウェブブラウザで表示するウェブページを作成するためのハイパーテキストマークアップ言語（HTML）を表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/web/htm/)で確認できます。 |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML（Hyper Text Markup Language）は、ブラウザで表示するウェブページの拡張子です。このファイル形式の詳細は[here](https://wiki.fileformat.com/web/html/)で確認できます。 |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | .ICO 拡張子のファイルは、Microsoft Windows 上でアプリケーションを表すアイコンとして使用される画像ファイルです。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/ico/)で確認できます。 |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000（J2C）は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を用いて設計され、JPEG 2000 は任意の品質でロスレスコンテンツを一度に符号化できます。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/jp2/)で確認できます。 |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000（J2K）は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を用いて設計され、JPEG 2000 は任意の品質でロスレスコンテンツを一度に符号化できます。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/jp2/)で確認できます。 |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000（JP2）は、画像符号化システムであり、最先端の画像圧縮規格です。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/jp2/)で確認できます。 |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000（JPC）は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を用いて設計され、JPEG 2000 は任意の品質でロスレスコンテンツを一度に符号化できます。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/jp2/)で確認できます。 |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG は、非可逆圧縮方式で保存される画像形式の一種です。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/jpeg/)で確認できます。 |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000（JPF）は、画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を用いて設計され、JPEG 2000 は任意の品質でロスレスコンテンツを一度に符号化できます。このファイル形式の詳細は[here](https://wiki.fileformat.com/image/jp2/)で確認できます。 |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG は、非可逆圧縮方式で保存される画像形式の一種です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/jpeg/)でご覧ください。 |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) は画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を用いて設計された JPEG 2000 は、任意の品質で無損失コンテンツを一度に符号化できます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/jp2/)でご覧ください。 |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) は画像符号化システムであり、最先端の画像圧縮規格です。ウェーブレット技術を用いて設計された JPEG 2000 は、任意の品質で無損失コンテンツを一度に符号化できます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/jp2/)でご覧ください。 |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | Markdown 言語方言で作成されたテキストファイルは、.MD または .MARKDOWN の拡張子で保存されます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/word-processing/md/)でご覧ください。 |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | MHT 拡張子のファイルは、さまざまなアプリケーションで作成できるウェブページアーカイブ形式を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/web/mhtml/)でご覧ください。 |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | MHTML 拡張子のファイルは、さまざまなアプリケーションで作成できるウェブページアーカイブ形式を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/web/mhtml/)でご覧ください。 |
| static readonly [MOBI](../../groupdocs.parser.options/filetype/mobi) | Mobipocket ファイル形式（もともとは .prc 拡張子、後に .mobi）は、電子書籍用の独自の、部分的に文書化されたバイナリ形式です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/ebook/mobi/)でご覧ください。 |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG は Microsoft Outlook および Exchange がメールメッセージ、連絡先、予定、その他のタスクを保存するために使用するファイル形式です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/email/msg/)でご覧ください。 |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | .numbers 拡張子を持つファイルは、Apple の iWork Numbers スプレッドシートアプリケーションで作成されたファイルです。 |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | ODG ファイル形式は、Apache OpenOffice の Draw アプリケーションでベクター画像として描画要素を保存するために使用されます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/odg/)でご覧ください。 |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | ODP 拡張子のファイルは、OpenOffice.org が OASIS Open 標準で使用するプレゼンテーションファイル形式を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/odp/)でご覧ください。 |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | ODS 拡張子のファイルは、ユーザーが編集可能な OpenDocument スプレッドシートドキュメント形式を指します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/spreadsheet/ods/)でご覧ください。 |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT ファイルは、OpenDocument テキストファイル形式に基づくワードプロセッサアプリケーションで作成される文書の一種です。無料の OpenOffice Writer などのワードプロセッサで作成され、テキスト、画像、オブジェクト、スタイルなどのコンテンツを保持できます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/word-processing/odt/)でご覧ください。 |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | .ONE 拡張子のファイルは Microsoft OneNote アプリケーションで作成されます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/note-taking/one/)でご覧ください。 |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST（オフラインストレージファイル）は、Microsoft Outlook を使用して Exchange Server に登録した際に、ローカルマシン上でオフラインモードのユーザーメールボックスデータを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/email/ost/)でご覧ください。 |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | .OTP 拡張子のファイルは、OASIS OpenDocument 標準形式で作成されたプレゼンテーションテンプレートファイルを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/otp/)でご覧ください。 |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS ファイルは、OpenOffice スプレッドシートアプリケーションで使用されるテンプレートファイルを含みます。 |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | OTT 拡張子のファイルは、OASIS の OpenDocument 標準形式に準拠してアプリケーションが生成するテンプレート文書を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/word-processing/ott/)でご覧ください。 |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL は Hewlett Packard (HP) が導入したページ記述言語である Printer Command Language の略です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/page-description-language/pcl/)でご覧ください。 |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | Portable Document Format（PDF）は、1990 年代に Adobe が作成した文書形式の一種です。このファイル形式の目的は、アプリケーションソフトウェア、ハードウェア、オペレーティングシステムに依存しない形で文書やその他の参照資料を表現する標準を導入することでした。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/view/pdf/)でご覧ください。 |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT ファイル形式は、ビットマップ画像とベクター画像の両方に使用できるメタフォーマットです。 |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG（Portable Network Graphics）は、ロスレス圧縮を使用するラスタ画像ファイル形式の一種です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/png/)でご覧ください。 |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | .POT 拡張子のファイルは、PowerPoint 97-2003 バージョンで作成された Microsoft PowerPoint テンプレートファイルを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/pot/)でご覧ください。 |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | POTM 拡張子のファイルは、マクロをサポートする Microsoft PowerPoint テンプレートファイルです。POTM ファイルは PowerPoint 2007 以降で作成され、今後のプレゼンテーションファイル作成に使用できる既定設定を含みます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/potm/)でご覧ください。 |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | .POTX 拡張子のファイルは、Microsoft PowerPoint 2007 以降で作成された Microsoft PowerPoint テンプレートプレゼンテーションを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/potx/)でご覧ください。 |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS、PowerPoint スライドショーは、Microsoft PowerPoint を使用してスライドショー目的で作成されます。PPS ファイルの読み取りと作成は Microsoft PowerPoint 97-2003 でサポートされています。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/pps/)。 |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | PPSM 拡張子のファイルは、Microsoft PowerPoint 2007 以降で作成されたマクロ対応スライドショー形式を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/ppsm/)。 |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX、PowerPoint スライドショーは、Microsoft PowerPoint 2007 以降を使用してスライドショー目的で作成されます。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/ppsx/)。 |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | PPT 拡張子のファイルは、スライドショーとして表示するためのスライド集合を含む PowerPoint ファイルを表します。これは Microsoft PowerPoint 97-2003 が使用するバイナリファイル形式を指定します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/ppt/)。 |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | PPTM 拡張子のファイルは、Microsoft PowerPoint 2007 以降のバージョンで作成されたマクロ対応プレゼンテーションファイルです。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/pptm/)。 |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | PPTX 拡張子のファイルは、広く使用されている Microsoft PowerPoint アプリケーションで作成されたプレゼンテーションファイルです。以前のバイナリ形式の PPT とは異なり、PPTX 形式は Microsoft PowerPoint のオープン XML プレゼンテーションファイル形式に基づいています。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/presentation/pptx/)。 |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) は、デスクトップおよび電子出版の分野で使用される汎用ページ記述言語です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/page-description-language/ps/)。 |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD、Photoshop Document は、Adobe Photoshop のグラフィック設計・開発に使用されるネイティブファイル形式を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/psd/)。 |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | .PST 拡張子のファイルは、Outlook の個人用ストレージファイル（Personal Storage Table とも呼ばれる）で、さまざまなユーザー情報を保存します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/email/pst/)。 |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | .rar 拡張子のファイルは、圧縮または非圧縮形式で情報を保存するために作成されたアーカイブファイルを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/compression/rar/)。 |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | Microsoft によって導入・文書化されたリッチテキスト形式 (RTF) は、アプリケーション内で使用するための書式付きテキストとグラフィックをエンコードする方法を表します。この形式は、他の Microsoft 製品とのクロスプラットフォーム文書交換を容易にし、相互運用性を実現します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/word-processing/rtf/)。 |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z は、高い圧縮率でファイルやフォルダーを圧縮するためのアーカイブ形式です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/compression/7z/)。 |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | SVG ファイルは、画像の外観を記述するために XML ベースのテキスト形式を使用するスカラーベクターグラフィックスファイルです。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/page-description-language/svg/)。 |
| static readonly [SVGZ](../../groupdocs.parser.options/filetype/svgz) | SVGZ ファイルは、画像の外観を記述するために XML ベースのテキスト形式を使用し、gzip 圧縮で圧縮されたスカラーベクターグラフィックスファイルです。 |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | .tar 拡張子のファイルは、1 つまたは複数のファイルをまとめるために Unix 系ユーティリティで作成されたアーカイブです。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/compression/tar/)。 |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | .TEXT 拡張子のファイルは、行単位のプレーンテキストを含むテキストドキュメントを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/word-processing/txt/)。 |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF、Tagged Image File Format は、このファイル形式標準に準拠したさまざまなデバイスでの使用を目的としたラスタ画像を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/tiff/)。 |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF、Tagged Image File Format は、このファイル形式標準に準拠したさまざまなデバイスでの使用を目的としたラスタ画像を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/tiff/)。 |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | タブ区切り値 (TSV) ファイル形式は、タブで区切られたプレーンテキスト形式のデータを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/spreadsheet/tsv/)。 |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | .TXT 拡張子のファイルは、行単位のプレーンテキストを含むテキストドキュメントを表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/word-processing/txt/)。 |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | 不明なファイルタイプを表します。 |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP は Google によって導入された、ロスレスおよびロッシー圧縮に基づく最新のラスタウェブ画像ファイル形式です。同等の画像品質を保ちつつ、画像サイズを大幅に削減します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/webp/)。 |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | WMF 拡張子のファイルは、ベクターとビットマップ形式の画像データを保存するための Microsoft Windows Metafile (WMF) を表します。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/image/wmf/)。 |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML は、XML 内のマークアップを使用し、HTML 4.0 を再定式化したテキストベースのファイル形式です。このファイル形式の詳細は[こちら](https://wiki.fileformat.com/web/xhtml/)。 |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | Excel 97-2003 アドインは、追加コードの実行を目的とした補助プログラムです。VBA プロジェクトの使用をサポートします。 |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | XMLベースでマクロ対応のAdd-In形式はExcel 2010およびExcel 2007用です。Add-Inは追加コードを実行するように設計された補助プログラムです。VBAプロジェクトとExcel 4.0マクロシート（.xlm）の使用をサポートします。 |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | XLS拡張子のファイルはExcel Binary File Formatを表します。このようなファイルはMicrosoft Excelだけでなく、OpenOffice CalcやApple Numbersなどの類似スプレッドシートプログラムでも作成できます。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xls/)で確認してください。 |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSBファイル形式はExcel Binary File Formatを指定し、これはExcelブックの内容を定義するレコードと構造のコレクションです。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xlsb/)で確認してください。 |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | XLSM拡張子のファイルはマクロをサポートするスプレッドシートファイルの一種です。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xlsm/)で確認してください。 |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSXはMicrosoft Office 2007のリリースとともにMicrosoftが導入した、Microsoft Excelドキュメントのよく知られた形式です。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xlsx/)で確認してください。 |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | .XLT拡張子のファイルは、Microsoft Officeスイートの一部であるスプレッドシートアプリケーションMicrosoft Excelで作成されたテンプレートファイルです。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xlt/)で確認してください。 |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM拡張子はMicrosoft Excelによって生成されるマクロ対応テンプレートファイルを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xltm/)で確認してください。 |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | XLTX拡張子のファイルはOffice OpenXMLファイル形式仕様に基づくMicrosoft Excelテンプレートファイルを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/specification/spreadsheet/xltx/)で確認してください。 |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XMLはExtensible Markup Languageの略で、HTMLに似ていますが、オブジェクトを定義するためにタグを使用する点が異なります。このファイル形式の詳細は[here](https://wiki.fileformat.com/web/xml/)で確認してください。 |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP拡張子は1つ以上のファイルやディレクトリを格納できるアーカイブを表します。このファイル形式の詳細は[here](https://wiki.fileformat.com/compression/zip/)で確認してください。 |

### 備考

**Learn more:**

* [Supported Document Formats](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [Get supported file formats](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
