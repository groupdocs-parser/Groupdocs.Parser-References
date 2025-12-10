---
title: TemplateLinkedPosition class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templatelinkedposition/
is_root: false
weight: 70
---

## TemplateLinkedPosition class

Provides a template field position which uses the linked field.



**Inheritance:** [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) → 
[`TemplatePosition`](/parser/python-net/groupdocs.parser.templates/templateposition)



The TemplateLinkedPosition type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/__init__/#System.String-groupdocs.parser.data.Size-groupdocs.parser.templates.TemplateLinkedPositionEdges) | Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) class. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/__init__/#System.String-groupdocs.parser.data.Size-groupdocs.parser.templates.TemplateLinkedPositionEdges-bool) | Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) class with UPPER CASE linked field name. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/__init__/#System.String-groupdocs.parser.data.Size-groupdocs.parser.templates.TemplateLinkedPositionEdges-bool-bool) | Initializes a new instance of the [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition) class. |


### Properties
| Property | Description |
| :- | :- |
| [linked_field_name](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/linked_field_name) | Gets the linked field name. |
| [search_area](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/search_area) | Gets the size of the area where a field is searched. |
| [edges](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/edges) | Gets the edges of the linked field where a field is searched. |
| [auto_scale](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/auto_scale) | Gets the value that indicates whether [`TemplateLinkedPosition.search_area`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition#search_area) is scaled by the linked field size. |



### Example 


The following example shows the code for the situation
if it's known that the field with an invoice number is placed on the right 
of "Invoice number" string the following code is used:

### See Also
* module [`groupdocs.parser.templates`](..)
* class [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition)
* class [`TemplatePosition`](/parser/python-net/groupdocs.parser.templates/templateposition)
