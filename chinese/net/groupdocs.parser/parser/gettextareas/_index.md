---
title: "GetTextAreas"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "从文档中提取文本区域。"
type: docs
weight: 190
url: /zh/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

从文档中提取文本区域。

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### 返回值

一个由[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)对象组成的集合；如果不支持文本区域提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 示例

下面的示例展示了如何从整个文档中提取所有文本区域：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 提取文本区域
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // 检查是否支持文本区域提取
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // 遍历页面文本区域
    foreach(PageTextArea a in areas)
    {
        // 打印页面索引、矩形和文本区域值：
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

使用自定义选项（正则表达式、区分大小写等）从文档中提取文本区域。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| options | PageTextAreaOptions | 文本区域提取的选项。 |

### 返回值

一个由[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)对象组成的集合；如果不支持文本区域提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 示例

下面的示例展示了如何仅从左上角提取包含数字的文本区域：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 创建用于文本区域提取的选项
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // 从页面的左上角提取仅包含数字的文本区域：
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // 检查是否支持文本区域提取
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // 遍历页面文本区域
    foreach(PageTextArea a in areas)
    {
        // 打印页面索引、矩形和文本区域值：
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

从文档页面提取文本区域。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |

### 返回值

一个由[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)对象组成的集合；如果不支持文本区域提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 示例

要从文档页面提取文本区域，使用以下方法：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 检查文档是否支持文本区域提取
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
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
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // 打印页面编号 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // 遍历页面文本区域
        // 我们忽略空值检查，因为我们之前已经检查了文本区域提取功能的支持情况
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // 打印矩形和文本区域值：
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

使用自定义选项（正则表达式、区分大小写等）从文档页面提取文本区域。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |
| options | PageTextAreaOptions | 文本区域提取的选项。 |

### 返回值

一个由[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)对象组成的集合；如果不支持文本区域提取，则为 `null`。

### 备注

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
