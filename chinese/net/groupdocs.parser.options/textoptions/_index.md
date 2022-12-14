---
title: TextOptions
second_title: GroupDocs.Parser for .NET API 参考
description: 提供用于文本提取的选项
type: docs
weight: 580
url: /zh/net/groupdocs.parser.options/textoptions/
---
## TextOptions class

提供用于文本提取的选项。

```csharp
public sealed class TextOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [TextOptions](textoptions)(bool) | 初始化[`TextOptions`](../textoptions)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; } | 获取指示是否使用原始模式的值。 |

### 评论

的一个实例[`TextOptions`](../textoptions)类用作 parameter in[`GetText`](../../groupdocs.parser/parser/gettext)和[`GetText`](../../groupdocs.parser/parser/gettext)方法。请参阅那里的用法示例。

用于指定文本提取的原始模式。 此模式下的文本提取方式不准确，但比标准模式下更快。 如果原始模式不支持文档格式，则忽略此参数，使用标准模式。

**学到更多：**

* [以准确模式提取文本](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [以原始模式提取文本](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 也可以看看

* 命名空间 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 部件 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
