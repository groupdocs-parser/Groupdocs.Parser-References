---
title: "TemplateTable"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "使用大写名称初始化 TemplateTablegroupdocs.parser.templates/templatetable 类的新实例。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

使用大写名称初始化 [`TemplateTable`](../../templatetable) 类的新实例。

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| layout | TemplateTableLayout | 表格布局。 |
| 名称 | 字符串 | 表格名称。 |

### 示例

如果无法自动检测表格，则通过表格布局设置模板表格：

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// 创建文档模板
Template template = new Template(new TemplateItem[] { table });
```

### 另请参见

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

使用大写名称初始化 [`TemplateTable`](../../templatetable) 类的新实例。

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| layout | TemplateTableLayout | 表格布局。 |
| 名称 | 字符串 | 表格名称。 |
| pageWidth | Nullable`1 | 用于创建模板项的页面宽度。 |

### 示例

如果无法自动检测表格，则通过表格布局设置模板表格：

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// 创建文档模板
Template template = new Template(new TemplateItem[] { table });
```

### 另请参见

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

初始化 [`TemplateTable`](../../templatetable) 类的新实例。

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| layout | TemplateTableLayout | 表格布局。 |
| 名称 | 字符串 | 表格名称。 |
| pageWidth | Nullable`1 | 用于创建模板项的页面宽度。 |
| useUpperCaseName | Boolean | 指示 `name` 是否被转换为大写的值。 |

### 示例

如果无法自动检测表格，则通过表格布局设置模板表格：

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// 创建文档模板
Template template = new Template(new TemplateItem[] { table });
```

### 另请参见

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

初始化 [`TemplateTable`](../../templatetable) 类的新实例。

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 参数 | TemplateTableParameters | 用于在自动模式下检测表格的参数。 |
| 名称 | 字符串 | 表格名称。 |

### 示例

如果通过检测器参数设置了模板表格，则表格会自动检测：

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// 创建文档模板
Template template = new Template(new TemplateItem[] { table });
```

### 另请参见

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

初始化 [`TemplateTable`](../../templatetable) 类的新实例。

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 参数 | TemplateTableParameters | 用于在自动模式下检测表格的参数。 |
| 名称 | 字符串 | 表格名称。 |
| pageWidth | Nullable`1 | 用于创建模板项的页面宽度。 |

### 示例

如果通过检测器参数设置了模板表格，则表格会自动检测：

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// 创建文档模板
Template template = new Template(new TemplateItem[] { table });
```

### 另请参见

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

初始化 [`TemplateTable`](../../templatetable) 类的新实例。

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 参数 | TemplateTableParameters | 用于在自动模式下检测表格的参数。 |
| 名称 | 字符串 | 表格名称。 |
| pageWidth | Nullable`1 | 用于创建模板项的页面宽度。 |
| useUpperCaseName | Boolean | 指示 `name` 是否被转换为大写的值。 |

### 示例

如果通过检测器参数设置了模板表格，则表格会自动检测：

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// 创建文档模板
Template template = new Template(new TemplateItem[] { table });
```

### 另请参见

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
