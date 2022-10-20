---
title: GetHyperlinks
second_title: GroupDocs.Parser for .NET API 参考
description: 从文档中提取超链接
type: docs
weight: 100
url: /zh/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

从文档中提取超链接。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### 返回值

集合[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)对象; `无效的`如果不支持超链接提取。

### 例子

以下示例展示了如何从整个文档中提取所有超链接：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持超链接提取
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // 从文档中提取超链接
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // 遍历超链接
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // 打印超链接文本
        Console.WriteLine(h.Text);
        // 打印超链接 URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 也可以看看

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

从文档页面中提取超链接。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 从零开始的页面索引。 |

### 返回值

集合[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)对象; `无效的`如果不支持超链接提取。

### 例子

下面的例子展示了如何从文档页面中提取超链接：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持超链接提取
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        //打印页码 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 从文档页面中提取超链接
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // 遍历超链接
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // 打印超链接文本
            Console.WriteLine(h.Text);
            // 打印超链接 URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### 也可以看看

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

使用自定义选项 （设置包含超链接的矩形区域）从文档中提取超链接。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| options | PageAreaOptions | 超链接提取的选项。 |

### 返回值

集合[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)对象; `无效的`如果不支持超链接提取。

### 例子

下面的例子展示了如何从文档页面区域中提取超链接：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持超链接提取
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // 创建用于超链接提取的选项
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // 从文档页面区域提取超链接
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // 遍历超链接
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // 打印超链接文本
        Console.WriteLine(h.Text);
        // 打印超链接 URL
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 也可以看看

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

使用自定义选项 （设置包含超链接的矩形区域）从文档页面中提取超链接。

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 从零开始的页面索引。 |
| options | PageAreaOptions | 超链接提取的选项。 |

### 返回值

集合[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea)对象; `无效的`如果不支持超链接提取。

### 例子

以下示例显示如何使用自定义选项从文档页面区域提取超链接：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持超链接提取
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
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
    
    // 创建用于超链接提取的选项
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // 遍历页面
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        //打印页码 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // 从文档页面区域提取超链接
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // 遍历超链接
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // 打印超链接文本
            Console.WriteLine(h.Text);
            // 打印超链接 URL
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### 也可以看看

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
