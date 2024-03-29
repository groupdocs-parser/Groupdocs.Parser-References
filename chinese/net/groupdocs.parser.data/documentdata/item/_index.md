---
title: Item
second_title: GroupDocs.Parser for .NET API 参考
description: 通过索引获取字段数据
type: docs
weight: 30
url: /zh/net/groupdocs.parser.data/documentdata/item/
---
## DocumentData indexer

通过索引获取字段数据。

```csharp
public FieldData this[int index] { get; }
```

| 范围 | 描述 |
| --- | --- |
| index | 字段的从零开始的索引。 |

### 返回值

的实例[`FieldData`](../../fielddata)班级。

### 例子

遍历所有字段：

[`FieldData`](../../fielddata)类代表字段数据。视领域而定[`PageArea`](../../fielddata/pagearea)property 可以包含的任何继承者[`PageArea`](../../pagearea)班级。例如，[`ParseForm`](../../../groupdocs.parser/parser/parseform) method 仅提取文本字段：

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

```csharp
// 创建解析器
using (Parser parser = new Parser(filePath))
{
    // 从 PDF 表单中提取数据
    DocumentData data = parser.ParseForm();
    // 遍历提取的字段
    for (int i = 0; i < data.Count; i++)
    {
        // 获取提取的字段
        FieldData field = data[i];
        // 打印字段名
        Console.Write(field.Name + ": ");
        // 检查字段值是否为文本并打印
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### 也可以看看

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* 命名空间 [GroupDocs.Parser.Data](../../documentdata)
* 部件 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
