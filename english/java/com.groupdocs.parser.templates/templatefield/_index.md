---
title: TemplateField
second_title: GroupDocs.Parser for Java API Reference
description: Provides the template text field.
type: docs
weight: 12
url: /java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Provides the template text field.

Text fields are defined by its position on the page. There are three ways to define a text field:

 *  Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
 *  Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
 *  Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Initializes a new instance of the [TemplateField](../../com.groupdocs.parser.templates/templatefield) class. |
| [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Initializes a new instance of the [TemplateField](../../com.groupdocs.parser.templates/templatefield) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPosition()](#getPosition--) | Gets the value that describes how to find the template field on the document page. |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Initializes a new instance of the [TemplateField](../../com.groupdocs.parser.templates/templatefield) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | The field position. |
| name | java.lang.String | The field name. |

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Initializes a new instance of the [TemplateField](../../com.groupdocs.parser.templates/templatefield) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | The field position. |
| name | java.lang.String | The field name. |
| pageIndex | java.lang.Integer | An integer value that represents the index of the page where the template item is located;  null  if the template item is located on any page. |

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Gets the value that describes how to find the template field on the document page.

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.
