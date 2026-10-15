---
title: "GetTables"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "从文档中提取表格。"
type: docs
weight: 170
url: /zh/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

从文档中提取表格。

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| options | PageTableAreaOptions | 表格提取的选项。 |

### 返回值

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 `null`。

### 示例

以下示例展示了如何从整个文档中提取表格：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持表格提取
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // 创建表格布局
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // 创建表格提取的选项
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // 从文档中提取表格
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // 遍历表
    foreach (PageTableArea t in tables)
    {
        // 遍历行
        for (int row = 0; row < t.RowCount; row++)
        {
            // 遍历列
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // 获取表格单元格
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // 打印表格单元格文本
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

从文档页面中提取表格。

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |
| options | PageTableAreaOptions | 表格提取的选项。 |

### 返回值

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 `null`。

### 示例

以下示例展示了如何从文档页中提取表格：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持表格提取
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // 创建表格布局
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // 创建表格提取的选项
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // 获取文档信息
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 检查文档是否有页面
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // 遍历页面
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // 打印页面编号 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 从文档页中提取表格
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // 遍历表
        foreach (PageTableArea t in tables)
        {
            // 遍历行
            for (int row = 0; row < t.RowCount; row++)
            {
                // 遍历列
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // 获取表格单元格
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // 打印表格单元格文本
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

从文档中提取表格。

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### 返回值

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 `null`。

### 示例

以下示例展示了如何从整个文档中提取表格：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持表格提取
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // 从文档中提取表格
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // 遍历表
    foreach (PageTableArea t in tables)
    {
        // 遍历行
        for (int row = 0; row < t.RowCount; row++)
        {
            // 遍历列
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // 获取表格单元格
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // 打印表格单元格文本
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

从文档页面中提取表格。

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |

### 返回值

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 对象的集合；如果不支持表格提取，则为 `null`。

### 示例

以下示例展示了如何从文档页中提取表格：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持表格提取
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // 获取文档信息
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 检查文档是否有页面
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // 遍历页面
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // 打印页面编号 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 从文档页中提取表格
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // 遍历表
        foreach (PageTableArea t in tables)
        {
            // 遍历行
            for (int row = 0; row < t.RowCount; row++)
            {
                // 遍历列
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // 获取表格单元格
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // 打印表格单元格文本
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
