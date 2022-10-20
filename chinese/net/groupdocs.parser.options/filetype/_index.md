---
title: FileType
second_title: GroupDocs.Parser for .NET API 参考
description: 表示文件类型提供方法来获取所支持的所有文件类型的列表GroupDocs.Parser.
type: docs
weight: 360
url: /zh/net/groupdocs.parser.options/filetype/
---
## FileType class

表示文件类型。提供方法来获取所支持的所有文件类型的列表**GroupDocs.Parser**.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | 文件名后缀（包括句点“.”） 例如“.doc”. |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | 文件类型名称，例如“Microsoft Word 文档”。 |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | 文件的格式，例如“WordProcessing”。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | 将文件扩展名映射到文件类型。 |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 判断当前是否[`FileType`](../filetype)与指定的相同[`FileType`](../filetype)对象. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 判断当前是否[`FileType`](../filetype)与指定对象相同。 |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 返回当前的哈希码[`FileType`](../filetype)对象. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 返回代表当前对象的字符串。 |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | 检索支持的文件类型 |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 判断两个[`FileType`](../filetype)对象是相同的。 |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 判断两个[`FileType`](../filetype)对象不一样。 |

## 字段

| 姓名 | 描述 |
| --- | --- |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | 扩展名为 .BMP 的文件表示位图图像文件，用于存储位图数字图像。 这些图像独立于图形适配器，也称为设备无关位图 (DIB) 文件 格式。了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/bmp/). |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | 使用 Bzip2 算法压缩的文件。 |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | 计算机图形元文件 (CGM) 是免费、独立于平台的国际标准元文件 格式，用于存储和交换矢量图形 (2D)、光栅图形和文本。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/page-description-language/cgm/). |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM 文件格式表示由 HTML 页面集合组成的 Microsoft HTML 帮助文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/chm/). |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | 带有 CSV（逗号分隔值）扩展名的文件表示纯文本文件 ，其中包含带有逗号分隔值的数据记录。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/spreadsheet/csv/). |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | 带有 .DCM 扩展名的文件代表数字图像，其中存储了患者的医学 信息，例如 MRI、CT 扫描和超声图像。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/image/dcm/). |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB（与设备无关的位图）文件是一种光栅图像文件，其结构 与标准位图文件 (BMP) 相似，但具有不同的标题。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/image/dib/). |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu，发音为“déjà vu”，是一种图形文件格式，适用于扫描文档和 书籍，尤其是包含文本、绘图、图像和照片组合的书籍。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/djvu/). |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | 带有.doc 扩展名的文件表示由Microsoft Word 或其他文字处理生成的文档 二进制文件格式的文档。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/doc/). |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM 文件是 Microsoft Word 2007 或更高版本生成的文档，能够运行宏。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/docm/). |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX 是一种众所周知的 Microsoft Word 文档格式。从 2007 年随 Microsoft Office 2007 的 release 引入，这种新文档格式的结构从普通的 binary 更改为 XML 和二进制文件的组合。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/docx/). |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | 带有 .DOT 扩展名的文件是由 Microsoft Word 创建的模板文件，具有预先格式化的设置 ，用于生成更多 DOC 或 DOCX 文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/dot/). |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | 带有 DOTM 扩展名的文件表示使用 Microsoft Word 2007 或更高版本创建的模板文件。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/dotm/). |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | 带有 DOTX 扩展名的文件是由 Microsoft Word 创建的模板文件，具有预先格式化的 settings 用于生成更多 DOCX 文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/dotx/). |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | 增强型元文件格式 (EMF) 独立于设备存储图形图像。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/image/emf/) |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML 文件格式表示使用 Outlook 和其他相关应用程序保存的电子邮件。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/email/eml/). |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX 文件格式由 Apple 实现和开发。 Apple Mail 应用程序使用 EMLX 文件格式导出电子邮件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/email/emlx/). |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | 带有 EPS 扩展名的文件本质上描述了一个 Encapsulated PostScript 语言程序 ，它描述了单个页面的外观。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/page-description-language/eps/). |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | 带有 .EPUB 扩展名的文件是一种电子书文件格式，它为出版商和消费者提供 一种标准的数字出版格式。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/ebook/epub/). |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | 带有 FB2 扩展名的文件是 FictionBook 2.0 电子书文件，其中包含电子书的结构。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/ebook/fb2/). |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF 或图形交换格式是一种高度压缩的图像。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/gif/). |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | .gz 扩展名的文件是使用 gzip 压缩应用程序创建的压缩文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/gz/). |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | 带有 HTM 扩展名的文件代表超文本标记语言，用于创建网页[这里](https://wiki.fileformat.com/web/htm/). |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML（超文本标记语言）是为在浏览器中显示而创建的网页的扩展。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/html/). |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | 带有 ICO 扩展名的文件是图像文件类型，用作在 Microsoft Windows 上表示应用程序的图标。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/ico/). |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000 (J2C) 是一种图像编码系统和最先进的图像压缩标准。设计， 使用小波技术 JPEG 2000 可以一次编码任何质量的无损内容。详细了解 这种文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000 (J2K) 是一种图像编码系统和最先进的图像压缩标准。设计， 使用小波技术 JPEG 2000 可以一次编码任何质量的无损内容。详细了解 这种文件格式[这里](https://wiki.fileformat.com/image/jp2/) |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000 (JP2) 是一种图像编码系统和最先进的图像压缩标准。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000 (JPC) 是一种图像编码系统和最先进的图像压缩标准。设计， 使用小波技术 JPEG 2000 可以一次编码任何质量的无损内容。详细了解 这种文件格式[这里](https://wiki.fileformat.com/image/jp2/) |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG 是一种使用有损压缩方法保存的图像格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000 (JPF) 是一种图像编码系统和最先进的图像压缩标准。设计， 使用小波技术 JPEG 2000 可以一次编码任何质量的无损内容。详细了解 这种文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG 是一种使用有损压缩方法保存的图像格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) 是一种图像编码系统和最先进的图像压缩标准。设计， 使用小波技术 JPEG 2000 可以一次编码任何质量的无损内容。详细了解 这种文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) 是一种图像编码系统和最先进的图像压缩标准。设计， 使用小波技术 JPEG 2000 可以一次编码任何质量的无损内容。详细了解 这种文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | 使用 Markdown 语言方言创建的文本文件以 .MD 或 .MARKDOWN 文件扩展名保存。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/md/). |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | 带有 MHT 扩展名的文件代表一种网页存档格式，可以由许多不同的应用程序创建 。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | 带有 MHTML 扩展名的文件代表一种网页存档格式，可以由许多不同的应用程序创建 。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG 是 Microsoft Outlook 和 Exchange 用于存储电子邮件、联系人、 约会或其他任务的文件格式。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/email/msg/). |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | 包含 .numbers 文件扩展名的文件是由 Apple iWork Numbers 电子表格应用程序创建的文件。 |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | Apache OpenOffice 的 Draw 应用程序使用 ODG 文件格式将 绘图元素存储为矢量图像。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/image/odg/). |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | 带有 ODP 扩展名的文件表示 OpenOffice.org 在 OASISOpen 标准中使用的演示文件格式。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/odp/). |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | 带有 ODS 扩展名的文件代表用户可编辑的 OpenDocument 电子表格文档格式。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/spreadsheet/ods/). |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT 文件是使用基于 OpenDocument 文本文件格式的文字处理应用程序创建的文档类型。这些是使用免费的 OpenOffice Writer 等文字处理器应用程序创建的， 可以保存文本、图像、对象和样式等内容。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/odt/). |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | .ONE 扩展名表示的文件由 Microsoft OneNote 应用程序创建。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/note-taking/one/). |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST 或脱机存储文件表示在使用 Microsoft Outlook 向 Exchange Server 注册后 在本地计算机上处于脱机模式的用户邮箱数据。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | 带有 .OTP 扩展名的文件表示由应用程序 以 OASIS OpenDocument 标准格式创建的演示模板文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/otp/). |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS 文件包含 OpenOffice 电子表格应用程序使用的模板文件。 |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | 带有 OTT 扩展名的文件表示由应用程序生成的模板文档，符合 OASIS 的 OpenDocument 标准格式。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/word-processing/ott/). |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL 代表打印机命令语言，它是由惠普 (HP) 推出的页面描述语言 。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/page-description-language/pcl/). |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | 可移植文档格式 (PDF) 是 Adobe 在 1990 年代创建的一种文档。 this 文件格式的目的是为文档和其他参考资料的表示引入一个标准，以 一种独立于应用软件、硬件和操作系统的格式。了解更多 关于这种文件格式[这里](https://wiki.fileformat.com/view/pdf/). |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT 文件格式是一种元格式，可用于位图图像和矢量图像。 |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG，便携式网络图形，是指一种使用无损压缩的光栅图像文件格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/png/). |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | 带有 .POT 扩展名的文件代表由 PowerPoint 97-2003 版本创建的 的 Microsoft PowerPoint 模板文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/pot/). |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | 带有 POTM 扩展名的文件是支持宏的 Microsoft PowerPoint 模板文件。 POTM files 是使用 PowerPoint 2007 或更高版本创建的，包含可用于创建 更多演示文件的默认设置。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/potm/). |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | 带有 .POTX 扩展名的文件表示使用 Microsoft PowerPoint 2007 及更高版本创建的 Microsoft PowerPoint 模板演示文稿。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/potx/). |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS，PowerPoint 幻灯片放映，文件是使用 Microsoft PowerPoint 创建的，用于幻灯片放映目的。 PPS 文件读取和创建受 Microsoft PowerPoint 97-2003 支持。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/pps/). |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | 带有 PPSM 扩展名的文件代表使用 Microsoft PowerPoint 2007 或更高版本创建的启用宏的幻灯片文件格式。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/ppsm/). |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX、Power Point 幻灯片放映文件是使用 Microsoft PowerPoint 2007 及更高版本为 幻灯片放映目的创建的。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/ppsx/). |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | 带有 PPT 扩展名的文件表示由幻灯片集合组成的 PowerPoint 文件， 显示为幻灯片。它指定 Microsoft PowerPoint 97-2003 使用的二进制文件格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/presentation/ppt/). |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | 带有 PPTM 扩展名的文件是使用 Microsoft PowerPoint 2007 或更高版本创建的启用宏的演示文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/pptm/). |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | 带有 PPTX 扩展名的文件是使用流行的 Microsoft PowerPoint 应用程序创建的演示文件。 与以前版本的二进制演示文件格式 PPT 不同，PPTX 格式基于 Microsoft PowerPoint 开放 XML 演示文件格式的 。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/presentation/pptx/). |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) 是一种通用的页面描述语言， 用于桌面和电子出版业务。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/page-description-language/ps/). |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD，Photoshop 文档，代表 Adobe Photoshop 的原生文件格式， 用于图形设计和开发。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/image/psd/). |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | 带有 .PST 扩展名的文件代表 Outlook 个人存储文件（也称为个人存储表） ，用于存储各种用户信息。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | .rar 扩展名的文件表示为以压缩或正常形式存储信息而创建的存档文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/rar/). |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | 由 Microsoft 引入和记录，富文本格式 (RTF) 代表了一种编码 格式化文本和图形以供在应用程序中使用的方法。该格式便于与其他 Microsoft 产品进行跨平台 document 交换，从而达到互操作性的目的。详细了解 这种文件格式[这里](https://wiki.fileformat.com/word-processing/rtf/). |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z 是一种用于压缩文件和文件夹的归档格式，具有高压缩比。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/7z/). |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | SVG 文件是一个标量矢量图形文件，它使用基于 XML 的文本格式 来描述图像的外观。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/page-description-language/svg/). |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | 带有 .tar 扩展名的文件是使用基于 Unix 的实用程序创建的存档，用于收集一个或多个文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/tar/). |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | 带有 .TEXT 扩展名的文件表示包含行形式的纯文本的文本文档。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF，标记图像文件格式，表示用于在符合此文件格式标准的各种 设备上使用的光栅图像。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF，标记图像文件格式，表示用于在符合此文件格式标准的各种 设备上使用的光栅图像。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | 制表符分隔值 (TSV) 文件格式表示用纯文本格式的制表符分隔的数据。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/spreadsheet/tsv/). |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | 带有 .TXT 扩展名的文件表示包含行形式的纯文本的文本文档。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | 表示未知文件类型。 |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP，由谷歌推出，是一种基于无损和 有损压缩的现代光栅网络图像文件格式。它提供相同的图像质量，同时显着减小图像大小。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/webp/). |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | 带有 WMF 扩展名的文件代表 Microsoft Windows 元文件 (WMF)，用于存储矢量 以及位图格式的图像数据。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/image/wmf/) |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML 是一种基于文本的文件格式，在 XML 中带有标记，使用 HTML 4.0 的重新表述。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/xhtml/). |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | Excel 97-2003 加载项，一个旨在运行附加代码的补充程序。 支持使用 VBA 项目。 |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | Excel 2010 和 Excel 2007 的基于 XML 且启用宏的加载项格式。 加载项是旨在运行附加代码的补充程序。 支持使用 VBA 项目和 Excel 4.0 宏表 (.xlm)。 |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | 带有 XLS 扩展名的文件代表 Excel 二进制文件格式。此类文件可由 Microsoft Excel 以及其他类似的电子表格程序（如 OpenOffice Calc 或 Apple Numbers）创建。详细了解 这种文件格式[这里](https://wiki.fileformat.com/specification/spreadsheet/xls/). |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB 文件格式指定 Excel 二进制文件格式，它是指定 Excel 工作簿内容的记录和 结构的集合。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/specification/spreadsheet/xlsb/). |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | 带有 XLSM 扩展名的文件是一种支持宏的电子表格文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/specification/spreadsheet/xlsm/). |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX 是 Microsoft Excel 文档的众所周知的格式，由 Microsoft 在 Microsoft Office 2007 的 release 中引入。了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/specification/spreadsheet/xlsx/). |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | 带有 .XLT 扩展名的文件是使用 Microsoft Excel 创建的模板文件，它是作为 Microsoft Office 套件的一部分提供的电子表格 应用程序。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/specification/spreadsheet/xlt/). |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM 文件扩展名将 Microsoft Excel 生成的文件表示为 Macro-enabled 模板文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/specification/spreadsheet/xltm/). |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | 带有 XLTX 扩展名的文件代表基于 Office OpenXML 文件格式规范的 Microsoft Excel 模板文件。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/specification/spreadsheet/xltx/). |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML 代表可扩展标记语言，它类似于 HTML ，但在使用标签定义对象方面有所不同。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/web/xml/). |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP 文件扩展名表示可以保存一个或多个文件或目录的档案。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/zip/). |

### 评论

**学到更多：**

* [支持的文档格式](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [获取支持的文件格式](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [获取文档信息](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 也可以看看

* 命名空间 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 部件 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
