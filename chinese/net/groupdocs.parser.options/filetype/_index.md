---
title: FileType
second_title: GroupDocs.Parser for .NET API 参考
description: 表示文件类型提供获取所有支持的文件类型列表的方法GroupDocs.解析器.
type: docs
weight: 380
url: /zh/net/groupdocs.parser.options/filetype/
---
## FileType class

表示文件类型。提供获取所有支持的文件类型列表的方法**GroupDocs.解析器**.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Extension](../../groupdocs.parser.options/filetype/extension) { get; } | 文件名后缀（包括句点“.”）例如“.doc”. |
| [FileFormat](../../groupdocs.parser.options/filetype/fileformat) { get; } | 文件类型名称，例如“Microsoft Word 文档”. |
| [Format](../../groupdocs.parser.options/filetype/format) { get; } | 文件格式，例如“WordProcessing”. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [FromExtension](../../groupdocs.parser.options/filetype/fromextension)(string) | 将文件扩展名映射到文件类型。 |
| [Equals](../../groupdocs.parser.options/filetype/equals#equals)(FileType) | 判断当前是否[`FileType`](../filetype)与指定的相同[`FileType`](../filetype)对象. |
| override [Equals](../../groupdocs.parser.options/filetype/equals#equals_1)(object) | 判断当前是否[`FileType`](../filetype)与指定对象相同。 |
| override [GetHashCode](../../groupdocs.parser.options/filetype/gethashcode)() | 返回当前的哈希码[`FileType`](../filetype)对象. |
| override [ToString](../../groupdocs.parser.options/filetype/tostring)() | 返回表示当前对象的字符串。 |
| static [GetSupportedFileTypes](../../groupdocs.parser.options/filetype/getsupportedfiletypes)() | 检索支持的文件类型 |
| [operator ==](../../groupdocs.parser.options/filetype/op_equality) | 判断是否两个[`FileType`](../filetype)对象是相同的。 |
| [operator !=](../../groupdocs.parser.options/filetype/op_inequality) | 判断是否两个[`FileType`](../filetype)对象不一样. |

## 字段

| 姓名 | 描述 |
| --- | --- |
| static readonly [BMP](../../groupdocs.parser.options/filetype/bmp) | 扩展名为 .BMP 的文件表示用于存储位图数字图像的位图图像文件。 这些图像独立于图形适配器，也称为设备独立位图 (DIB) 文件 格式。了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/bmp/). |
| static readonly [BZ2](../../groupdocs.parser.options/filetype/bz2) | 使用 Bzip2 算法的压缩文件。 |
| static readonly [CGM](../../groupdocs.parser.options/filetype/cgm) | 计算机图形图元文件 (CGM) 是免费的、独立于平台的国际标准图元文件 格式，用于存储和交换矢量图形 (2D)、光栅图形和文本。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/page-description-language/cgm/). |
| static readonly [CHM](../../groupdocs.parser.options/filetype/chm) | CHM 文件格式表示由 HTML 页面集合组成的 Microsoft HTML 帮助文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/chm/). |
| static readonly [CSV](../../groupdocs.parser.options/filetype/csv) | 具有 CSV（逗号分隔值）扩展名的文件代表纯文本文件 ，其中包含具有逗号分隔值的数据记录。详细了解此文件格式 [这里](https://wiki.fileformat.com/spreadsheet/csv/). |
| static readonly [DCM](../../groupdocs.parser.options/filetype/dcm) | 扩展名为 .DCM 的文件代表数字图像，它存储患者的医学 信息，例如 MRI、CT 扫描和超声图像。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/image/dcm/). |
| static readonly [DIB](../../groupdocs.parser.options/filetype/dib) | DIB（设备独立位图）文件是一种光栅图像文件，其结构 与标准位图文件 (BMP) 相似，但标头不同。详细了解此文件格式 [这里](https://wiki.fileformat.com/image/dib/). |
| static readonly [DJVU](../../groupdocs.parser.options/filetype/djvu) | DjVu，发音为“déjà vu”，是一种图形文件格式，用于扫描文档和 书籍，尤其是那些包含文本、绘图、图像和照片组合的书籍。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/djvu/). |
| static readonly [DOC](../../groupdocs.parser.options/filetype/doc) | 扩展名为 .doc 的文件表示由 Microsoft Word 或其他文字处理生成的文档， 二进制文件格式的文档。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/doc/). |
| static readonly [DOCM](../../groupdocs.parser.options/filetype/docm) | DOCM 文件是 Microsoft Word 2007 或更高版本生成的文档，能够运行宏。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/docm/). |
| static readonly [DOCX](../../groupdocs.parser.options/filetype/docx) | DOCX 是一种众所周知的 Microsoft Word 文档格式。从 2007 年随 Microsoft Office 2007 的 release 引入，这种新文档格式的结构从普通的 binary 更改为 XML 和二进制文件的组合。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/docx/). |
| static readonly [DOT](../../groupdocs.parser.options/filetype/dot) | 扩展名为 .DOT 的文件是由 Microsoft Word 创建的模板文件，具有预格式化设置 用于生成更多 DOC 或 DOCX 文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/dot/). |
| static readonly [DOTM](../../groupdocs.parser.options/filetype/dotm) | 带有 DOTM 扩展名的文件表示使用 Microsoft Word 2007 或更高版本创建的模板文件。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/dotm/). |
| static readonly [DOTX](../../groupdocs.parser.options/filetype/dotx) | 具有 DOTX 扩展名的文件是由 Microsoft Word 创建的模板文件，具有预格式化设置 用于生成更多 DOCX 文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/dotx/). |
| static readonly [EMF](../../groupdocs.parser.options/filetype/emf) | 增强型图元文件格式 (EMF) 独立于设备存储图形图像。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/image/emf/) |
| static readonly [EML](../../groupdocs.parser.options/filetype/eml) | EML 文件格式表示使用 Outlook 和其他相关应用程序保存的电子邮件。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/email/eml/). |
| static readonly [EMLX](../../groupdocs.parser.options/filetype/emlx) | EMLX 文件格式由 Apple 实施和开发。 Apple Mail 应用程序使用 EMLX 文件格式导出电子邮件。详细了解此文件格式 [这里](https://wiki.fileformat.com/email/emlx/). |
| static readonly [EPS](../../groupdocs.parser.options/filetype/eps) | 具有 EPS 扩展名的文件本质上描述了一个封装的 PostScript 语言程序 ，它描述了单个页面的外观。详细了解此文件格式 [这里](https://wiki.fileformat.com/page-description-language/eps/). |
| static readonly [EPUB](../../groupdocs.parser.options/filetype/epub) | 扩展名为 .EPUB 的文件是一种电子书文件格式，它为出版商和消费者提供 标准数字出版物格式。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/ebook/epub/). |
| static readonly [FB2](../../groupdocs.parser.options/filetype/fb2) | 具有 FB2 扩展名的文件是包含电子书结构的 FictionBook 2.0 电子书文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/ebook/fb2/). |
| static readonly [GIF](../../groupdocs.parser.options/filetype/gif) | GIF 或图形交换格式是一种高度压缩的图像。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/gif/). |
| static readonly [GZ](../../groupdocs.parser.options/filetype/gz) | 扩展名为 .gz 的文件是使用 gzip 压缩应用程序创建的压缩文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/gz/). |
| static readonly [HTM](../../groupdocs.parser.options/filetype/htm) | 具有 HTM 扩展名的文件表示用于创建网页的超文本标记语言 用于在网络浏览器（例如 Google Chrome、Internet Explorer、Firefox 和其他一些浏览器）中显示。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/htm/). |
| static readonly [HTML](../../groupdocs.parser.options/filetype/html) | HTML（超文本标记语言）是为在浏览器中显示而创建的网页的扩展。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/html/). |
| static readonly [ICO](../../groupdocs.parser.options/filetype/ico) | 带 ICO 扩展名的文件是用作图标的图像文件类型，用于表示 Microsoft Windows 上的应用程序。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/ico/). |
| static readonly [J2C](../../groupdocs.parser.options/filetype/j2c) | JPEG 2000 (J2C) 是图像编码系统和最先进的图像压缩标准。 使用小波技术设计的 JPEG 2000 可以一次对任何质量的无损内容进行编码。详细了解 此文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [J2K](../../groupdocs.parser.options/filetype/j2k) | JPEG 2000 (J2K) 是图像编码系统和最先进的图像压缩标准。 使用小波技术设计的 JPEG 2000 可以一次对任何质量的无损内容进行编码。详细了解 此文件格式[这里](https://wiki.fileformat.com/image/jp2/) |
| static readonly [JP2](../../groupdocs.parser.options/filetype/jp2) | JPEG 2000 (JP2) 是一种图像编码系统和最先进的图像压缩标准。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPC](../../groupdocs.parser.options/filetype/jpc) | JPEG 2000 (JPC) 是图像编码系统和最先进的图像压缩标准。 使用小波技术设计的 JPEG 2000 可以一次对任何质量的无损内容进行编码。详细了解 此文件格式[这里](https://wiki.fileformat.com/image/jp2/) |
| static readonly [JPEG](../../groupdocs.parser.options/filetype/jpeg) | JPEG 是一种使用有损压缩方法保存的图像格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPF](../../groupdocs.parser.options/filetype/jpf) | JPEG 2000 (JPF) 是一种图像编码系统和最先进的图像压缩标准。 使用小波技术设计的 JPEG 2000 可以一次对任何质量的无损内容进行编码。详细了解 此文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPG](../../groupdocs.parser.options/filetype/jpg) | JPG 是一种使用有损压缩方法保存的图像格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/jpeg/). |
| static readonly [JPM](../../groupdocs.parser.options/filetype/jpm) | JPEG 2000 (JPM) 是图像编码系统和最先进的图像压缩标准。 使用小波技术设计的 JPEG 2000 可以一次对任何质量的无损内容进行编码。详细了解 此文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [JPX](../../groupdocs.parser.options/filetype/jpx) | JPEG 2000 (JPX) 是一种图像编码系统和最先进的图像压缩标准。 使用小波技术设计的 JPEG 2000 可以一次对任何质量的无损内容进行编码。详细了解 此文件格式[这里](https://wiki.fileformat.com/image/jp2/). |
| static readonly [MD](../../groupdocs.parser.options/filetype/md) | 使用 Markdown 语言方言创建的文本文件以 .MD 或 .MARKDOWN 文件扩展名保存。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/md/). |
| static readonly [MHT](../../groupdocs.parser.options/filetype/mht) | 具有 MHT 扩展名的文件代表一种网页存档格式，可以由许多不同的应用程序创建 。详细了解此文件格式 [这里](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MHTML](../../groupdocs.parser.options/filetype/mhtml) | 具有 MHTML 扩展名的文件代表一种网页存档格式，可以由许多不同的应用程序创建 。详细了解此文件格式 [这里](https://wiki.fileformat.com/web/mhtml/). |
| static readonly [MSG](../../groupdocs.parser.options/filetype/msg) | MSG 是 Microsoft Outlook 和 Exchange 用于存储电子邮件、联系人、 约会或其他任务的文件格式。详细了解此文件格式 [这里](https://wiki.fileformat.com/email/msg/). |
| static readonly [NUMBERS](../../groupdocs.parser.options/filetype/numbers) | 包含 .numbers 文件扩展名的文件是由 Apple iWork Numbers 电子表格应用程序创建的文件。 |
| static readonly [ODG](../../groupdocs.parser.options/filetype/odg) | Apache OpenOffice 的 Draw 应用程序使用 ODG 文件格式将 绘图元素存储为矢量图像。详细了解此文件格式 [这里](https://wiki.fileformat.com/image/odg/). |
| static readonly [ODP](../../groupdocs.parser.options/filetype/odp) | 具有 ODP 扩展名的文件表示 OpenOffice.org 在 OASISOpen 标准中使用的演示文件格式。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/odp/). |
| static readonly [ODS](../../groupdocs.parser.options/filetype/ods) | 带有 ODS 扩展名的文件代表用户可编辑的 OpenDocument 电子表格文档格式。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/spreadsheet/ods/). |
| static readonly [ODT](../../groupdocs.parser.options/filetype/odt) | ODT 文件是使用基于 OpenDocument 文本文件格式的文字处理应用程序创建的文档类型。这些是使用文字处理器应用程序创建的，例如免费的 OpenOffice Writer 和 可以保存文本、图像、对象和样式等内容。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/odt/). |
| static readonly [ONE](../../groupdocs.parser.options/filetype/one) | .ONE 扩展名表示的文件由 Microsoft OneNote 应用程序创建。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/note-taking/one/). |
| static readonly [OST](../../groupdocs.parser.options/filetype/ost) | OST 或脱机存储文件表示用户在使用 Microsoft Outlook 向 Exchange Server 注册 时在脱机模式下在本地计算机上的邮箱数据。详细了解此文件格式 [这里](https://wiki.fileformat.com/email/ost/) |
| static readonly [OTP](../../groupdocs.parser.options/filetype/otp) | 扩展名为 .OTP 的文件表示由应用程序 创建的 OASIS OpenDocument 标准格式的演示文稿模板文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/otp/). |
| static readonly [OTS](../../groupdocs.parser.options/filetype/ots) | OTS 文件包含 OpenOffice 电子表格应用程序使用的模板文件。 |
| static readonly [OTT](../../groupdocs.parser.options/filetype/ott) | 具有 OTT 扩展名的文件代表应用程序生成的模板文档，符合 OASIS 的 OpenDocument 标准格式。详细了解此文件格式 [这里](https://wiki.fileformat.com/word-processing/ott/). |
| static readonly [PCL](../../groupdocs.parser.options/filetype/pcl) | PCL 代表 Printer Command Language 是一种页面描述语言 由惠普 (HP) 推出。详细了解此文件格式 [这里](https://wiki.fileformat.com/page-description-language/pcl/). |
| static readonly [PDF](../../groupdocs.parser.options/filetype/pdf) | 便携式文档格式 (PDF) 是 Adobe 在 1990 年代创建的一种文档。 this 文件格式的目的是在 中引入文档和其他参考资料的表示标准，这是一种独立于应用程序软件、硬件和操作系统的格式。了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/view/pdf/). |
| static readonly [PICT](../../groupdocs.parser.options/filetype/pict) | PICT 文件格式是一种元格式，可用于位图图像和矢量图像。 |
| static readonly [PNG](../../groupdocs.parser.options/filetype/png) | PNG，便携式网络图形，指的是一种使用无损压缩的光栅图像文件格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/png/). |
| static readonly [POT](../../groupdocs.parser.options/filetype/pot) | 带有 .POT 扩展名的文件代表由 PowerPoint 97-2003 版本创建的 Microsoft PowerPoint 模板文件 。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/pot/). |
| static readonly [POTM](../../groupdocs.parser.options/filetype/potm) | 带有 POTM 扩展名的文件是支持宏的 Microsoft PowerPoint 模板文件。 POTM 文件 是使用 PowerPoint 2007 或更高版本创建的，包含可用于创建 更多演示文稿文件的默认设置。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/potm/). |
| static readonly [POTX](../../groupdocs.parser.options/filetype/potx) | 带有 .POTX 扩展名的文件表示使用 Microsoft PowerPoint 2007 及更高版本创建的 Microsoft PowerPoint 模板演示文稿。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/potx/). |
| static readonly [PPS](../../groupdocs.parser.options/filetype/pps) | PPS、PowerPoint 幻灯片，文件是使用 Microsoft PowerPoint 为幻灯片放映目的创建的。 Microsoft PowerPoint 97-2003 支持读取和创建 PPS 文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/pps/). |
| static readonly [PPSM](../../groupdocs.parser.options/filetype/ppsm) | 带有 PPSM 扩展名的文件表示使用 Microsoft PowerPoint 2007 或更高版本创建的启用宏的幻灯片放映文件格式。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/ppsm/). |
| static readonly [PPSX](../../groupdocs.parser.options/filetype/ppsx) | PPSX、Power Point 幻灯片放映文件是使用 Microsoft PowerPoint 2007 及更高版本创建的，用于 幻灯片放映目的。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/ppsx/). |
| static readonly [PPT](../../groupdocs.parser.options/filetype/ppt) | 带有 PPT 扩展名的文件代表 PowerPoint 文件，它由一组显示为 SlideShow 的幻灯片 for 组成。它指定 Microsoft PowerPoint 97-2003 使用的二进制文件格式。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/presentation/ppt/). |
| static readonly [PPTM](../../groupdocs.parser.options/filetype/pptm) | 具有 PPTM 扩展名的文件是使用 Microsoft PowerPoint 2007 或更高版本创建的启用宏的演示文稿文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/pptm/). |
| static readonly [PPTX](../../groupdocs.parser.options/filetype/pptx) | 带有 PPTX 扩展名的文件是使用流行的 Microsoft PowerPoint 应用程序创建的演示文稿文件。 与以前版本的二进制演示文稿文件格式 PPT 不同，PPTX 格式基于 Microsoft PowerPoint open XML 演示文稿文件格式。详细了解此文件格式 [这里](https://wiki.fileformat.com/presentation/pptx/). |
| static readonly [PS](../../groupdocs.parser.options/filetype/ps) | PostScript (PS) 是一种通用页面描述语言， 用于桌面和电子出版业务。详细了解此文件格式 [这里](https://wiki.fileformat.com/page-description-language/ps/). |
| static readonly [PSD](../../groupdocs.parser.options/filetype/psd) | PSD，Photoshop 文档，代表 Adobe Photoshop 的本机文件格式，用于 图形设计和开发。详细了解此文件格式 [这里](https://wiki.fileformat.com/image/psd/). |
| static readonly [PST](../../groupdocs.parser.options/filetype/pst) | 扩展名为 .PST 的文件代表 Outlook 个人存储文件（也称为个人存储表） ，它存储各种用户信息。详细了解此文件格式 [这里](https://wiki.fileformat.com/email/pst/) |
| static readonly [RAR](../../groupdocs.parser.options/filetype/rar) | 具有 .rar 扩展名的文件表示为以压缩或正常形式存储信息而创建的存档文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/rar/). |
| static readonly [RTF](../../groupdocs.parser.options/filetype/rtf) | 富文本格式 (RTF) 由 Microsoft 引入并记录在案，代表了一种编码 格式的文本和图形以在应用程序中使用的方法。该格式便于与其他 Microsoft 产品进行跨平台 document 交换，从而达到互操作性的目的。详细了解 此文件格式[这里](https://wiki.fileformat.com/word-processing/rtf/). |
| static readonly [SEVENZ](../../groupdocs.parser.options/filetype/sevenz) | 7z 是一种以高压缩比压缩文件和文件夹的归档格式。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/7z/). |
| static readonly [SVG](../../groupdocs.parser.options/filetype/svg) | SVG 文件是一种标量矢量图形文件，它使用基于 XML 的文本格式 来描述图像的外观。详细了解此文件格式 [这里](https://wiki.fileformat.com/page-description-language/svg/). |
| static readonly [TAR](../../groupdocs.parser.options/filetype/tar) | 扩展名为 .tar 的文件是使用基于 Unix 的实用程序创建的存档，用于收集一个或多个文件。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/tar/). |
| static readonly [TEXT](../../groupdocs.parser.options/filetype/text) | 具有 .TEXT 扩展名的文件表示包含行形式的纯文本的文本文档。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [TIF](../../groupdocs.parser.options/filetype/tif) | TIF，标记图像文件格式，表示用于各种 符合此文件格式标准的设备的光栅图像。详细了解此文件格式 [这里](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TIFF](../../groupdocs.parser.options/filetype/tiff) | TIFF，标记图像文件格式，表示用于各种 符合此文件格式标准的设备的光栅图像。详细了解此文件格式 [这里](https://wiki.fileformat.com/image/tiff/). |
| static readonly [TSV](../../groupdocs.parser.options/filetype/tsv) | 制表符分隔值 (TSV) 文件格式表示以纯文本格式的制表符分隔的数据。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/spreadsheet/tsv/). |
| static readonly [TXT](../../groupdocs.parser.options/filetype/txt) | 扩展名为 .TXT 的文件表示包含行形式的纯文本的文本文档。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/word-processing/txt/). |
| static readonly [Unknown](../../groupdocs.parser.options/filetype/unknown) | 代表未知文件类型。 |
| static readonly [WEBP](../../groupdocs.parser.options/filetype/webp) | WebP，由谷歌推出，是一种基于无损和 有损压缩的现代光栅网络图像文件格式。它提供相同的图像质量，同时显着减小图像大小。 了解有关此文件格式的更多信息[这里](https://wiki.fileformat.com/image/webp/). |
| static readonly [WMF](../../groupdocs.parser.options/filetype/wmf) | 具有 WMF 扩展名的文件表示用于存储矢量 以及位图格式图像数据的 Microsoft Windows 图元文件 (WMF)。详细了解此文件格式 [这里](https://wiki.fileformat.com/image/wmf/) . |
| static readonly [XHTML](../../groupdocs.parser.options/filetype/xhtml) | XHTML 是一种基于文本的文件格式，在 XML 中带有标记，使用 HTML 4.0 的重新表述。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/web/xhtml/). |
| static readonly [XLA](../../groupdocs.parser.options/filetype/xla) | Excel 97-2003 加载项，一个旨在运行附加代码的补充程序。 支持使用 VBA 项目。 |
| static readonly [XLAM](../../groupdocs.parser.options/filetype/xlam) | Excel 2010 和 Excel 2007 的基于 XML 和启用宏的加载项格式。 加载项是一种补充程序，旨在运行其他代码。 支持使用 VBA 项目和 Excel 4.0 宏表 (.xlm)。 |
| static readonly [XLS](../../groupdocs.parser.options/filetype/xls) | 具有 XLS 扩展名的文件代表 Excel 二进制文件格式。此类文件可以由 Microsoft Excel 以及其他类似的电子表格程序（例如 OpenOffice Calc 或 Apple Numbers）创建。详细了解 此文件格式[这里](https://wiki.fileformat.com/specification/spreadsheet/xls/). |
| static readonly [XLSB](../../groupdocs.parser.options/filetype/xlsb) | XLSB 文件格式指定 Excel 二进制文件格式，它是指定 Excel 工作簿内容的记录和 结构的集合。详细了解此文件格式 [这里](https://wiki.fileformat.com/specification/spreadsheet/xlsb/). |
| static readonly [XLSM](../../groupdocs.parser.options/filetype/xlsm) | 具有 XLSM 扩展名的文件是一种支持宏的 Spreasheet 文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/specification/spreadsheet/xlsm/). |
| static readonly [XLSX](../../groupdocs.parser.options/filetype/xlsx) | XLSX 是众所周知的 Microsoft Excel 文档格式，由 Microsoft 在 Microsoft Office 2007 的 版本中引入。了解有关此文件格式 的更多信息[这里](https://wiki.fileformat.com/specification/spreadsheet/xlsx/). |
| static readonly [XLT](../../groupdocs.parser.options/filetype/xlt) | 扩展名为 .XLT 的文件是使用 Microsoft Excel 创建的模板文件，Microsoft Excel 是一个电子表格 应用程序，是 Microsoft Office 套件的一部分。详细了解此文件格式 [这里](https://wiki.fileformat.com/specification/spreadsheet/xlt/). |
| static readonly [XLTM](../../groupdocs.parser.options/filetype/xltm) | XLTM 文件扩展名表示由 Microsoft Excel 生成的文件，作为启用宏的 模板文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/specification/spreadsheet/xltm/). |
| static readonly [XLTX](../../groupdocs.parser.options/filetype/xltx) | 具有 XLTX 扩展名的文件表示基于 Office OpenXML 文件格式规范的 Microsoft Excel 模板文件。详细了解此文件格式 [这里](https://wiki.fileformat.com/specification/spreadsheet/xltx/). |
| static readonly [XML](../../groupdocs.parser.options/filetype/xml) | XML 是Extensible Markup Language 的缩写，与HTML 类似，但不同的是使用标签来定义对象。详细了解此文件格式 [这里](https://wiki.fileformat.com/web/xml/). |
| static readonly [ZIP](../../groupdocs.parser.options/filetype/zip) | ZIP 文件扩展名表示可以保存一个或多个文件或目录的档案。 了解有关此文件格式的更多信息 [这里](https://wiki.fileformat.com/compression/zip/). |

### 评论

**了解更多：**

* [支持的文档格式](https://docs.groupdocs.com/display/parsernet/Supported+Document+Formats)
* [获取支持的文件格式](https://docs.groupdocs.com/display/parsernet/Get+supported+file+formats)
* [获取文档信息](https://docs.groupdocs.com/display/parsernet/Get+document+info)

### 也可以看看

* 命名空间 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 部件 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
