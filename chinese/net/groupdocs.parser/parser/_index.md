---
title: Parser
second_title: GroupDocs.Parser for .NET API 参考
description: 表示控制文本图像容器提取和解析功能的主类
type: docs
weight: 590
url: /zh/net/groupdocs.parser/parser/
---
## Parser class

表示控制文本、图像、容器提取和解析功能的主类。

```csharp
public sealed class Parser : IDisposable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | 初始化[`Parser`](../parser)类从数据库中提取数据。 |
| [Parser](parser#constructor)(EmailConnection) | 初始化[`Parser`](../parser)从远程电子邮件服务器中提取数据的类。 |
| [Parser](parser#constructor_4)(Stream) | 初始化[`Parser`](../parser)类. |
| [Parser](parser#constructor_7)(string) | 初始化[`Parser`](../parser)类. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | 初始化[`Parser`](../parser)类从数据库中提取数据。 |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | 初始化[`Parser`](../parser)从远程电子邮件服务器中提取数据的类。 |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | 初始化[`Parser`](../parser)类与[`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_8)(string, LoadOptions) | 初始化[`Parser`](../parser)类与[`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | 初始化[`Parser`](../parser)类与[`LoadOptions`](../../groupdocs.parser.options/loadoptions) 和[`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions, ParserSettings) | 初始化[`Parser`](../parser)类与[`LoadOptions`](../../groupdocs.parser.options/loadoptions) 和[`ParserSettings`](../../groupdocs.parser.options/parsersettings). |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | 获取支持的功能。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | 执行与释放、释放或重置非托管资源相关的应用程序定义任务。 |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | 获取页面预览。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | 从文档中提取条形码。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | 从文档页面中提取条形码。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | 使用自定义选项 从文档中提取条形码（设置包含条形码的矩形区域）。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | 使用自定义选项 （设置包含条形码的矩形区域）从文档页面中提取条形码。 |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | 从文档中提取容器对象以使用包含附件、ZIP 存档等的格式。 |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | 返回有关文档的一般信息。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | 从文档中提取格式化文本。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | 从文档页面中提取格式化文本。 |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | 从文档中提取亮点。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | 从文档中提取超链接。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | 从文档页面中提取超链接。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | 使用自定义选项 （设置包含超链接的矩形区域）从文档中提取超链接。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | 使用自定义选项 （设置包含超链接的矩形区域）从文档页面中提取超链接。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | 从文档中提取图像。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | 从文档页面中提取图像。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | 使用自定义选项 （设置包含图像的矩形区域）从文档中提取图像。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | 使用自定义选项 （设置包含图像的矩形区域）从文档页面中提取图像。 |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | 从文档中提取元数据。 |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | 从文档中提取结构化文本。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | 从文档中提取表格。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | 从文档页面中提取表格。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | 从文档中提取文本。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | 从文档页面中提取文本。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | 使用文本选项从文档中提取文本页面（以启用原始快速文本提取模式）。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | 使用文本选项从文档页面中提取文本（以启用原始快速文本提取模式）。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | 从文档中提取文本区域。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | 从文档页面中提取文本区域。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | 使用自定义选项（正则表达式、匹配大小写等）从文档中提取文本区域。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | 使用自定义选项（正则表达式、匹配大小写等）从文档页面中提取文本区域。 |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | 从文档中提取目录。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | 通过用户生成的模板解析文档。 |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | 解析文档表单。 |
| [Search](../../groupdocs.parser/parser/search#search)(string) | 搜索一个*keyword*在文档中。 |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | 搜索一个*keyword*在文档中使用搜索选项（正则表达式、匹配大小写等）。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | 返回有关文件的一般信息。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | 返回有关文件的一般信息。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | 返回有关文件的一般信息。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | 返回有关文件的一般信息。 |

### 也可以看看

* 命名空间 [GroupDocs.Parser](../../groupdocs.parser)
* 部件 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
