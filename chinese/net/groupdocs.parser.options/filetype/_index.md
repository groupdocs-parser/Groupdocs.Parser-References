---
title: "FileType"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "表示文件类型。提供获取 GroupDocs.Parser 支持的所有文件类型列表的方法。"
type: docs
weight: 320
url: /zh/net/groupdocs.parser.options/filetype/
---

## FileType class

表示文件类型。提供获取 **GroupDocs.Parser** 支持的所有文件类型列表的方法。

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | 文件名后缀（包括句点 \".\"），例如 \".doc\"。 |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | 文件类型名称，例如 \"Microsoft Word Document\"。 |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | 文件格式，例如 \"WordProcessing\"。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | 将文件扩展名映射到文件类型。 |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 确定当前的 [`FileType`](../filetype) 是否与指定的 [`FileType`](../filetype) 对象相同。 |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 确定当前的 [`FileType`](../filetype) 是否与指定的对象相同。 |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 返回当前 [`FileType`](../filetype) 对象的哈希码。 |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 返回表示当前对象的字符串。 |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | 检索受支持的文件类型 |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 确定两个 [`FileType`](../filetype) 对象是否相同。 |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 确定两个 [`FileType`](../filetype) 对象是否不相同。 |

## 字段

| 名称 | 描述 |
| --- | --- |
| static readonly [AZW3](../../groupdocs.parser.options/filetype/azw3) | AZW3，也称为 Kindle Format 8 (KF8)，是为 Amazon Kindle 设备开发的 AZW 电子书数字文件格式的改进版。了解更多关于此文件格式的信息，请点击[此处](https://wiki.fileformat.com/ebook/azw3/)。 |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | 扩展名为 .BMP 的文件表示用于存储位图数字图像的位图图像文件。这些图像独立于图形适配器，也称为设备无关位图（DIB）文件格式。了解更多关于此文件格式的信息，请点击[此处](https://wiki.fileformat.com/image/bmp/)。 |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | 使用 Bzip2 算法压缩的文件。 |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | Computer Graphics Metafile (CGM) 是一种免费、平台无关的国际标准元文件格式，用于存储和交换矢量图形（2D）、光栅图形和文本。了解更多关于此文件格式的信息，请点击[此处](https://wiki.fileformat.com/page-description-language/cgm/)。 |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM 文件格式表示由一系列 HTML 页面组成的 Microsoft HTML 帮助文件。了解更多关于此文件格式的信息，请点击[此处](https://wiki.fileformat.com/web/chm/)。 |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | 扩展名为 CSV（逗号分隔值）的文件表示包含逗号分隔数据记录的纯文本文件。了解更多关于此文件格式的信息，请点击[此处](https://wiki.fileformat.com/spreadsheet/csv/)。 |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | 扩展名为 .DCM 的文件表示用于存储患者医学信息（如 MRI、CT 扫描和超声图像）的数字图像。了解更多关于此文件格式的信息，请点击[此处](https://wiki.fileformat.com/image/dcm/)。 |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB（Device Independent Bitmap）文件是一种光栅图像文件，其结构类似于标准位图文件（BMP），但具有不同的标题。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/dib/)。 |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu，发音为“déjà vu”，是一种用于扫描文档和书籍的图形文件格式，尤其适用于包含文本、图形、图像和照片组合的文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/djvu/)。 |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | 带有 .doc 扩展名的文件表示由 Microsoft Word 或其他文字处理程序生成的二进制文件格式文档。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/doc/)。 |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM 文件是由 Microsoft Word 2007 或更高版本生成的、具备运行宏功能的文档。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/docm/)。 |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX 是一种广为人知的 Microsoft Word 文档格式。自 2007 年 Microsoft Office 2007 发布起，引入了该新文档格式，其结构从纯二进制更改为 XML 与二进制文件的组合。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/docx/)。 |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | 带有 .DOT 扩展名的文件是 Microsoft Word 创建的模板文件，用于预先设置格式，以便生成后续的 DOC 或 DOCX 文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/dot/)。 |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | 带有 DOTM 扩展名的文件是由 Microsoft Word 2007 或更高版本创建的模板文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/dotm/)。 |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | 带有 .DOTX 扩展名的文件是 Microsoft Word 创建的模板文件，用于预先设置格式，以便生成后续的 DOCX 文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/dotx/)。 |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | 增强型图元文件格式（EMF）以设备无关的方式存储图形图像。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/emf/)。 |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML 文件格式表示使用 Outlook 及其他相关应用程序保存的电子邮件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/email/eml/)。 |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX 文件格式由 Apple 实现和开发。Apple Mail 应用程序使用 EMLX 文件格式导出电子邮件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/email/emlx/)。 |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | 带有 EPS 扩展名的文件本质上描述了一个封装的 PostScript 语言程序，用于描绘单页的外观。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/page-description-language/eps/)。 |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | 带有 .EPUB 扩展名的文件是一种电子书文件格式，为出版商和读者提供标准的数字出版格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/ebook/epub/)。 |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | 带有 FB2 扩展名的文件是 FictionBook 2.0 电子书文件，包含电子书的结构。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/ebook/fb2/)。 |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF（图形交换格式）是一种高度压缩的图像类型。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/gif/)。 |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | 带有 .gz 扩展名的文件是使用 gzip 压缩应用程序创建的压缩文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/compression/gz/)。 |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | 带有 HTM 扩展名的文件代表用于创建网页的超文本标记语言，可在 Google Chrome、Internet Explorer、Firefox 等浏览器中显示。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/web/htm/)。 |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML（超文本标记语言）是用于创建在浏览器中显示的网页的扩展名。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/web/html/)。 |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | 带有 ICO 扩展名的文件是用于在 Microsoft Windows 上表示应用程序图标的图像文件类型。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/ico/)。 |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000（J2C）是一种图像编码系统和先进的图像压缩标准。采用小波技术设计，JPEG 2000 能一次性对任何质量的内容进行无损编码。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000（J2K）是一种图像编码系统和先进的图像压缩标准。采用小波技术设计，JPEG 2000 能一次性对任何质量的内容进行无损编码。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000（JP2）是一种图像编码系统和先进的图像压缩标准。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000（JPC）是一种图像编码系统和先进的图像压缩标准。采用小波技术设计，JPEG 2000 能一次性对任何质量的内容进行无损编码。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG 是一种使用有损压缩方法保存的图像格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jpeg/)。 |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000（JPF）是一种图像编码系统和先进的图像压缩标准。采用小波技术设计，JPEG 2000 能一次性对任何质量的内容进行无损编码。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG 是一种使用有损压缩方法保存的图像格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jpeg/)。 |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) 是一种图像编码系统和最先进的图像压缩标准。采用小波技术设计，JPEG 2000 能一次性以任意质量对无损内容进行编码。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) 是一种图像编码系统和最先进的图像压缩标准。采用小波技术设计，JPEG 2000 能一次性以任意质量对无损内容进行编码。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/jp2/)。 |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | 使用 Markdown 语言方言创建的文本文件以 .MD 或 .MARKDOWN 文件扩展名保存。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/md/)。 |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | 带有 MHT 扩展名的文件表示一种网页存档格式，可由多种不同的应用程序创建。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/web/mhtml/)。 |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | 带有 MHTML 扩展名的文件表示一种网页存档格式，可由多种不同的应用程序创建。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/web/mhtml/)。 |
| static readonly [MOBI](../../groupdocs.parser.options/filetype/mobi) | Mobipocket 文件格式（最初使用 .prc 扩展名，后改为 .mobi）是一种专有的、部分文档化的二进制电子书格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/ebook/mobi/)。 |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG 是 Microsoft Outlook 和 Exchange 用于存储电子邮件、联系人、约会或其他任务的文件格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/email/msg/)。 |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | 带有 .numbers 扩展名的文件是由 Apple iWork Numbers 电子表格应用程序创建的文件。 |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | ODG 文件格式被 Apache OpenOffice 的 Draw 应用程序用于以矢量图像存储绘图元素。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/odg/)。 |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | 带有 ODP 扩展名的文件表示 OpenOffice.org 在 OASIS Open 标准中使用的演示文稿文件格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/presentation/odp/)。 |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | 带有 ODS 扩展名的文件代表可由用户编辑的 OpenDocument 电子表格文档格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/spreadsheet/ods/)。 |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT 文件是一种基于 OpenDocument 文本文档格式的文字处理应用程序创建的文档。这些文件由诸如免费 OpenOffice Writer 等文字处理软件创建，可包含文本、图像、对象和样式等内容。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/odt/)。 |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | 带有 .ONE 扩展名的文件由 Microsoft OneNote 应用程序创建。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/note-taking/one/)。 |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST（离线存储文件）表示用户在使用 Microsoft Outlook 注册 Exchange Server 后，在本地机器上离线模式下的邮箱数据。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/email/ost/)。 |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | 带有 .OTP 扩展名的文件表示使用 OASIS OpenDocument 标准格式创建的演示文稿模板文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/presentation/otp/)。 |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS 文件包含 OpenOffice 电子表格应用程序使用的模板文件。 |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | 带有 OTT 扩展名的文件表示符合 OASIS OpenDocument 标准格式的应用程序生成的模板文档。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/word-processing/ott/)。 |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL 代表由惠普（HP）推出的页面描述语言——打印机命令语言。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/page-description-language/pcl/)。 |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | 便携式文档格式（PDF）是一种由 Adobe 在 1990 年代创建的文档类型。该文件格式的目的是引入一种独立于应用软件、硬件以及操作系统的文档和其他参考材料的表示标准。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/view/pdf/)。 |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT 文件格式是一种可用于位图图像和矢量图像的元格式。 |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG（可移植网络图形）是指一种使用无损压缩的光栅图像文件格式。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/image/png/)。 |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | 带有 .POT 扩展名的文件表示由 PowerPoint 97-2003 版本创建的 Microsoft PowerPoint 模板文件。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/presentation/pot/)。 |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | 带有 POTM 扩展名的文件是支持宏的 Microsoft PowerPoint 模板文件。POTM 文件由 PowerPoint 2007 及以上版本创建，包含可用于创建后续演示文稿的默认设置。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/presentation/potm/)。 |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | 带有 .POTX 扩展名的文件表示由 Microsoft PowerPoint 2007 及以上版本创建的 Microsoft PowerPoint 模板演示文稿。了解更多关于此文件格式的信息，请点击[here](https://wiki.fileformat.com/presentation/potx/)。 |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS，PowerPoint 幻灯片放映文件，是使用 Microsoft PowerPoint 为放映目的创建的。Microsoft PowerPoint 97-2003 支持 PPS 文件的读取和创建。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/presentation/pps/). |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | 带有 PPSM 扩展名的文件表示使用 Microsoft PowerPoint 2007 或更高版本创建的支持宏的幻灯片放映文件格式。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/presentation/ppsm/). |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX，Power Point 幻灯片放映文件，是使用 Microsoft PowerPoint 2007 及以上版本为放映目的创建的。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/presentation/ppsx/). |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | 扩展名为 PPT 的文件表示 PowerPoint 文件，包含一系列用于幻灯片放映的幻灯片。它指定了 Microsoft PowerPoint 97-2003 使用的二进制文件格式。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/presentation/ppt/). |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | 带有 PPTM 扩展名的文件是使用 Microsoft PowerPoint 2007 或更高版本创建的支持宏的演示文稿文件。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/presentation/pptm/). |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | 带有 PPTX 扩展名的文件是使用流行的 Microsoft PowerPoint 应用程序创建的演示文稿文件。与之前的二进制 PPT 演示文稿文件格式不同，PPTX 格式基于 Microsoft PowerPoint 开放 XML 演示文稿文件格式。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/presentation/pptx/). |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript（PS）是一种通用页面描述语言，广泛用于桌面和电子出版业务。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/page-description-language/ps/). |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD，Photoshop 文档，代表 Adobe Photoshop 的原生文件格式，用于图形设计和开发。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/image/psd/). |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | 带有 .PST 扩展名的文件表示 Outlook 个人存储文件（亦称个人存储表），用于存储各种用户信息。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | 带有 .rar 扩展名的文件是为以压缩或普通形式存储信息而创建的归档文件。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/compression/rar/). |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | 由 Microsoft 引入并记录的富文本格式（RTF）是一种用于在应用程序中编码格式化文本和图形的方法。该格式促进了与其他 Microsoft 产品的跨平台文档交换，从而实现互操作性。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/word-processing/rtf/). |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z 是一种用于高压缩比压缩文件和文件夹的归档格式。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/compression/7z/). |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | SVG 文件是一种可缩放矢量图形文件，使用基于 XML 的文本格式描述图像的外观。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/page-description-language/svg/). |
| static readonly [SVGZ](../../groupdocs.parser.options/filetype/svgz) | SVGZ 文件是一种可缩放矢量图形文件，使用基于 XML 的文本格式描述图像的外观，并通过 gzip 压缩。 |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | 带有 .tar 扩展名的文件是使用基于 Unix 的工具创建的归档，用于收集一个或多个文件。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/compression/tar/). |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | 扩展名为 .TEXT 的文件表示包含逐行纯文本的文本文档。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF，标记图像文件格式，表示用于各种符合此文件格式标准的设备上的光栅图像。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF，标记图像文件格式，表示用于各种符合此文件格式标准的设备上的光栅图像。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | 制表符分隔值（TSV）文件格式表示以制表符分隔的纯文本数据。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/spreadsheet/tsv/). |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | 扩展名为 .TXT 的文件表示包含逐行纯文本的文本文档。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | 表示未知文件类型。 |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP 由 Google 推出，是一种基于无损和有损压缩的现代光栅网络图像文件格式。它在显著减小图像大小的同时提供相同的图像质量。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/image/webp/). |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | 带有 WMF 扩展名的文件表示 Microsoft Windows 元文件（WMF），用于存储矢量以及位图格式的图像数据。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/image/wmf/). |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML 是一种基于 XML 标记的文本文件格式，使用 HTML 4.0 的重新表述。了解更多关于此文件格式的信息[here](https://wiki.fileformat.com/web/xhtml/). |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | Excel 97-2003 加载项是一个补充程序，旨在运行额外代码。支持使用 VBA 项目。 |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | 基于 XML 且支持宏的 Excel 2010 和 Excel 2007 的 Add-In 格式。Add-In 是一种补充程序，旨在运行额外的代码。支持使用 VBA 项目和 Excel 4.0 宏工作表（.xlm）。 |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | 带有 XLS 扩展名的文件表示 Excel 二进制文件格式。这类文件可以由 Microsoft Excel 以及其他类似的电子表格程序（如 OpenOffice Calc 或 Apple Numbers）创建。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xls/)。 |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB 文件格式指定了 Excel 二进制文件格式，它是一组记录和结构，用于定义 Excel 工作簿的内容。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xlsb/)。 |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | 带有 XLSM 扩展名的文件是一种支持宏的电子表格文件。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xlsm/)。 |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX 是一种广为人知的 Microsoft Excel 文档格式，随 Microsoft Office 2007 的发布而由 Microsoft 引入。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xlsx/)。 |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | 带有 .XLT 扩展名的文件是使用 Microsoft Excel 创建的模板文件，Excel 是 Microsoft Office 套件中的电子表格应用程序。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xlt/)。 |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM 文件扩展名表示由 Microsoft Excel 生成的宏启用模板文件。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xltm/)。 |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | 带有 XLTX 扩展名的文件是基于 Office OpenXML 文件格式规范的 Microsoft Excel 模板文件。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/specification/spreadsheet/xltx/)。 |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML 代表可扩展标记语言，它类似于 HTML，但在使用标签定义对象方面有所不同。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/web/xml/)。 |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP 文件扩展名表示可以容纳一个或多个文件或目录的压缩档案。了解更多关于此文件格式的信息，请访问[此处](https://wiki.fileformat.com/compression/zip/)。 |

### 备注

**Learn more:**

* [Supported Document Formats](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [Get supported file formats](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 另请参见

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
