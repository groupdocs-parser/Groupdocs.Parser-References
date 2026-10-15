---
title: "解析器"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "表示控制文本图像容器提取和解析功能的主类。"
type: docs
weight: 30
url: /zh/net/groupdocs.parser/parser/
---

## Parser class

表示控制文本、图像、容器提取和解析功能的主类。

```csharp
public sealed class Parser : IDisposable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | 初始化 [`Parser`](../parser) 类的新实例，以从数据库提取数据。 |
| [Parser](parser#constructor)(EmailConnection) | 初始化 [`Parser`](../parser) 类的新实例，以从远程电子邮件服务器提取数据。 |
| [Parser](parser#constructor_4)(Stream) | 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_8)(string) | 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_12)(Uri) | 初始化 [`Parser`](../parser) 类的新实例，以从 URI 提取数据。 |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | 初始化 [`Parser`](../parser) 类的新实例，以从数据库提取数据。 |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | 初始化 [`Parser`](../parser) 类的新实例，以从远程电子邮件服务器提取数据。 |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | 使用 [`LoadOptions`](../../groupdocs.parser.options/loadoptions) 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | 使用 [`ParserSettings`](../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_9)(string, LoadOptions) | 使用 [`LoadOptions`](../../groupdocs.parser.options/loadoptions) 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_11)(string, ParserSettings) | 使用 [`ParserSettings`](../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | 初始化 [`Parser`](../parser) 类的新实例，以使用 *loadOptions* 从 URI 提取数据。 |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | 初始化 [`Parser`](../parser) 类的新实例，以使用 *parserSettings* 从 URI 提取数据。 |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | 使用 [`LoadOptions`](../../groupdocs.parser.options/loadoptions) 和 [`ParserSettings`](../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | 使用 [`LoadOptions`](../../groupdocs.parser.options/loadoptions) 和 [`ParserSettings`](../../groupdocs.parser.options/parsersettings) 初始化 [`Parser`](../parser) 类的新实例。 |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | 初始化 [`Parser`](../parser) 类的新实例，以使用 *loadOptions* 和 *parserSettings* 从 URI 提取数据。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | 获取受支持的功能。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | 执行与释放、释放或重置非托管资源相关的应用程序定义任务。 |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | 生成用于自动调整模板位置和比例的字段。 |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | 获取页面预览。 |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | 从文档中提取注释。请注意，目前仅支持 PDF 格式。 |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | 从文档页面中提取注释。请注意，目前仅支持 PDF 格式。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | 从文档中提取条形码。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | 使用自定义选项从文档中提取条形码。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | 从文档页面中提取条形码。 |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | 使用自定义选项从文档页面中提取条形码。 |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | 从文档中提取容器对象，以处理包含附件、ZIP 存档等的格式。 |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | 返回关于文档的一般信息。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | 从文档中提取格式化文本。 |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | 从文档页面中提取格式化文本。 |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | 从文档中提取高亮。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | 从文档中提取超链接。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | 从文档页面中提取超链接。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | 使用自定义选项从文档中提取超链接（用于设置包含超链接的矩形区域）。 |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | 使用自定义选项从文档页面中提取超链接（用于设置包含超链接的矩形区域）。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | 从文档中提取图像。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | 从文档页面中提取图像。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | 使用自定义选项从文档中提取图像（用于设置包含图像的矩形区域）。 |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | 使用自定义选项从文档页面中提取图像（用于设置包含图像的矩形区域）。 |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | 从文档中提取元数据。 |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | 生成文档页面预览。 |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | 使用自定义选项生成文档页面预览。 |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | 从文档中提取结构化文本。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | 从文档中提取表格。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | 从文档页面中提取表格。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | 从文档中提取表格。 |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | 从文档页面中提取表格。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | 从文档中提取文本。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | 从文档页面中提取文本。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | 使用文本选项从文档中提取文本页（以启用原始快速文本提取模式）。 |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | 使用文本选项从文档页面提取文本（以启用原始快速文本提取模式）。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | 从文档中提取文本区域。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | 从文档页面提取文本区域。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | 使用自定义选项（正则表达式、区分大小写等）从文档中提取文本区域。 |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | 使用自定义选项（正则表达式、区分大小写等）从文档页面提取文本区域。 |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | 从文档中提取目录。 |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | 提取工作表单元格。 |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | 使用自定义选项提取工作表单元格。 |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | 提取电子表格中所有工作表的信息。 |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | 提取工作表的信息。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | 使用用户生成的模板解析文档。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | 使用自定义选项通过用户生成的模板解析文档。 |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | 从提供的集合中选择最合适的模板，然后使用所选模板解析文档。 |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | 解析文档表单。 |
| [Search](../../groupdocs.parser/parser/search#search)(string) | 在文档中搜索 *keyword*。 |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | 使用搜索选项（正则表达式、区分大小写等）在文档中搜索 *keyword*。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | 返回有关文件的一般信息。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | 返回有关文件的一般信息。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | 返回有关文件的一般信息。 |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | 返回有关文件的一般信息。 |

### 另请参见

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
