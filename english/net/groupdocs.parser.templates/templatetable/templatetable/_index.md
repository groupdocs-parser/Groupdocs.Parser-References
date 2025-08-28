---
title: TemplateTable
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the TemplateTablegroupdocs.parser.templates/templatetable class with the UPPER CASE name.
type: docs
weight: 10
url: /net/groupdocs.parser.templates/templatetable/templatetable/
---
## TemplateTable(TemplateTableLayout, string) {#constructor}

Initializes a new instance of the [`TemplateTable`](../../templatetable) class with the UPPER CASE name.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| layout | TemplateTableLayout | The table layout. |
| name | String | The table name. |

### Examples

Template table is set by table layout if the table can't be detected automatically:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Create a document template
Template template = new Template(new TemplateItem[] { table });
```

### See Also

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Initializes a new instance of the [`TemplateTable`](../../templatetable) class with the UPPER CASE name.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | Description |
| --- | --- | --- |
| layout | TemplateTableLayout | The table layout. |
| name | String | The table name. |
| pageWidth | Nullable`1 | The width of the page that was used to create the template item. |

### Examples

Template table is set by table layout if the table can't be detected automatically:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Create a document template
Template template = new Template(new TemplateItem[] { table });
```

### See Also

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Initializes a new instance of the [`TemplateTable`](../../templatetable) class.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| layout | TemplateTableLayout | The table layout. |
| name | String | The table name. |
| pageWidth | Nullable`1 | The width of the page that was used to create the template item. |
| useUpperCaseName | Boolean | The value that indicates whether a `name` is converted to UPPER CASE. |

### Examples

Template table is set by table layout if the table can't be detected automatically:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Create a document template
Template template = new Template(new TemplateItem[] { table });
```

### See Also

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Initializes a new instance of the [`TemplateTable`](../../templatetable) class.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| parameters | TemplateTableParameters | The parameters to detect the table in the automatic mode. |
| name | String | The table name. |

### Examples

If a template table is set by detector parameters, the table is detected automatically:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Create a document template
Template template = new Template(new TemplateItem[] { table });
```

### See Also

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Initializes a new instance of the [`TemplateTable`](../../templatetable) class.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | Description |
| --- | --- | --- |
| parameters | TemplateTableParameters | The parameters to detect the table in the automatic mode. |
| name | String | The table name. |
| pageWidth | Nullable`1 | The width of the page that was used to create the template item. |

### Examples

If a template table is set by detector parameters, the table is detected automatically:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Create a document template
Template template = new Template(new TemplateItem[] { table });
```

### See Also

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Initializes a new instance of the [`TemplateTable`](../../templatetable) class.

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| parameters | TemplateTableParameters | The parameters to detect the table in the automatic mode. |
| name | String | The table name. |
| pageWidth | Nullable`1 | The width of the page that was used to create the template item. |
| useUpperCaseName | Boolean | The value that indicates whether a `name` is converted to UPPER CASE. |

### Examples

If a template table is set by detector parameters, the table is detected automatically:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Create a document template
Template template = new Template(new TemplateItem[] { table });
```

### See Also

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
