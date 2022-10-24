---
title: PageTextAreaOptions
second_title: GroupDocs.Parser for .NET API 参考
description: 提供用于页面文本区域提取的选项
type: docs
weight: 500
url: /zh/net/groupdocs.parser.options/pagetextareaoptions/
---
## PageTextAreaOptions class

提供用于页面文本区域提取的选项。

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)(string) | 初始化[`PageTextAreaOptions`](../pagetextareaoptions)使用正则表达式的类。 其他选项默认设置（详见备注） |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(string, Rectangle) | 初始化[`PageTextAreaOptions`](../pagetextareaoptions) class 带有正则表达式和矩形区域。 其他选项默认设置（详见备注） |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(string, bool, bool, bool, Rectangle) | 初始化[`PageTextAreaOptions`](../pagetextareaoptions)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; } | 获取正则表达式。 |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; } | 获取指示是否忽略文本格式的值。 |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; } | 获取指示是否不忽略文本大小写的值。 |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; } | 获取包含页面区域的矩形区域。 |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; } | 获取表示段是否合并的值。 |

### 评论

的一个实例[`PageTextAreaOptions`](../pagetextareaoptions)类用作参数 [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)和[`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)方法. 请参阅那里的用法示例。 **学到更多：**

* [提取文本区域](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 也可以看看

* class [PageAreaOptions](../pageareaoptions)
* 命名空间 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 部件 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->