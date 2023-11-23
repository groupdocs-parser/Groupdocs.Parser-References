---
title: TemplateTable
second_title: GroupDocs.Parser for Java API Reference
description: Provides the template table.
type: docs
weight: 20
url: /java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Provides the template table.

There are two ways to define a table:

 *  Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
 *  Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class with the UPPER CASE name. |
| [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class. |
| [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class with the UPPER CASE name. |
| [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLayout()](#getLayout--) | Gets the table layout. |
| [getParameters()](#getParameters--) | Gets the parameters to detect the table in the automatic mode. |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class with the UPPER CASE name.

Template table is set by table layout if the table can't be detected automatically:

```
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | The table layout. |
| name | java.lang.String | The table name. |
| pageIndex | java.lang.Integer | The index of the page where the template table is located;  null  if the template table is located on any page. |

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | The table layout. |
| name | java.lang.String | The table name. |
| pageIndex | java.lang.Integer | The index of the page where the template table is located;  null  if the template table is located on any page. |
| useUpperCaseName | boolean | The value that indicates whether a  name  is converted to UPPER CASE. |

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class with the UPPER CASE name.

If a template table is set by detector parameters, the table is detected automatically:

```
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | The parameters to detect the table in the automatic mode. |
| name | java.lang.String | The table name. |
| pageIndex | java.lang.Integer | The index of the page where the template table is located;  null  if the template table is located on any page. |

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initializes a new instance of the [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | The parameters to detect the table in the automatic mode. |
| name | java.lang.String | The table name. |
| pageIndex | java.lang.Integer | The index of the page where the template table is located;  null  if the template table is located on any page. |
| useUpperCaseName | boolean | The value that indicates whether a  name  is converted to UPPER CASE. |

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Gets the table layout.

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.
### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Gets the parameters to detect the table in the automatic mode.

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.
