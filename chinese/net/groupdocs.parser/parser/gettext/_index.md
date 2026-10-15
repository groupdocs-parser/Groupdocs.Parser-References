---
title: "GetText"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "从文档中提取文本。"
type: docs
weight: 180
url: /zh/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

从文档中提取文本。

```csharp
public TextReader GetText()
```

### 返回值

具有提取文本的 TextReader 类实例；如果不支持文本提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 示例

以下示例展示如何从文档中提取文本：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 将文本提取到读取器中
    using(TextReader reader = parser.GetText())
    {
        // 打印文档中的文本
        // 如果不支持文本提取，reader 为 null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 另请参见

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

使用文本选项从文档中提取文本页（以启用原始快速文本提取模式）。

```csharp
public TextReader GetText(TextOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| options | TextOptions | 文本提取选项。 |

### 返回值

具有提取文本的 TextReader 类实例；如果不支持文本提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 示例

下面的示例展示了如何从文档中提取原始文本：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 将原始文本提取到 reader 中
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // 打印文档中的文本
        // 如果不支持文本提取，reader 为 null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 另请参见

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

从文档页面中提取文本。

```csharp
public TextReader GetText(int pageIndex)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |

### 返回值

TextReader 类的实例，包含提取的文本；如果不支持文本页提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 示例

下面的示例展示了如何从文档页中提取文本：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 检查文档是否支持文本提取
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // 获取文档信息
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 检查文档是否有页面
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // 遍历页面
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // 打印页面编号 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // 将文本提取到读取器中
        using(TextReader reader = parser.GetText(p))
        {
            // 打印文档中的文本
            // 我们忽略 null 检查，因为我们已经提前检查了文本提取功能的支持情况
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 另请参见

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

使用文本选项从文档页面提取文本（以启用原始快速文本提取模式）。

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |
| options | TextOptions | 文本提取选项。 |

### 返回值

TextReader 类的实例，包含提取的文本；如果不支持文本页提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 示例

下面的示例展示了如何从文档页中提取原始文本：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 检查文档是否支持文本提取
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // 获取文档信息
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // 检查文档是否有页面
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // 遍历页面
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // 打印页面编号 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // 将文本提取到读取器中
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // 打印文档中的文本
            // 我们忽略 null 检查，因为我们已经提前检查了文本提取功能的支持情况
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 另请参见

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
