---
title: GetFormattedText
second_title: GroupDocs.Parser for .NET API 参考
description: 从文档中提取格式化文本
type: docs
weight: 80
url: /zh/net/groupdocs.parser/parser/getformattedtext/
---
## GetFormattedText(FormattedTextOptions) {#getformattedtext}

从文档中提取格式化文本。

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| options | FormattedTextOptions | 格式化文本提取选项。 |

### 返回值

的一个实例TextReader提取文本的类； `无效的`如果不支持格式化文本提取。

### 评论

**学到更多：**

* [从文档中提取格式化文本](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* 提取文档文本为[HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* 提取文档文本为[降价](https://docs.groupdocs.com/display/parsernet/Markdown)
* 提取文档文本为[纯文本](https://docs.groupdocs.com/display/parsernet/Plain+text)

### 例子

以下示例显示如何将文档文本提取为 HTML 文本：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 将格式化的文本提取到阅读器中
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // 打印文档中的格式化文本
        // 如果不支持格式化文本提取，则 reader 为 null
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### 也可以看看

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

从文档页面中提取格式化文本。

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 从零开始的页面索引。 |
| options | FormattedTextOptions | 格式化文本提取选项。 |

### 返回值

的一个实例TextReader提取文本的类； `无效的`如果不支持格式化文本页面提取。

### 评论

**学到更多：**

* [从文档页面中提取格式化文本](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* 提取文档文本为[HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* 提取文档文本为[降价](https://docs.groupdocs.com/display/parsernet/Markdown)
* 提取文档文本为[纯文本](https://docs.groupdocs.com/display/parsernet/Plain+text)

### 例子

以下示例显示如何将文档页面文本提取为 Markdown 文本：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持格式化文本提取
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
        return;
    }
    
    // 获取文档信息
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 检查文档是否有页面
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // 遍历页面
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        //打印页码 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // 将格式化的文本提取到阅读器中
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // 打印文档中的格式化文本
            // 我们忽略空值检查，因为我们之前检查了格式化文本提取功能支持
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 也可以看看

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->