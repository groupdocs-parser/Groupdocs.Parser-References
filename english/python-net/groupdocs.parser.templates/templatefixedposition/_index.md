---
title: TemplateFixedPosition class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templatefixedposition/
is_root: false
weight: 50
---

## TemplateFixedPosition class

Provides a template field position which is defined by the rectangular area.



**Inheritance:** [`TemplateFixedPosition`](/parser/python-net/groupdocs.parser.templates/templatefixedposition) → 
[`TemplatePosition`](/parser/python-net/groupdocs.parser.templates/templateposition)



The TemplateFixedPosition type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatefixedposition/__init__/#groupdocs.parser.data.Rectangle) | Initializes a new instance of the [`TemplateFixedPosition`](/parser/python-net/groupdocs.parser.templates/templatefixedposition) class. |


### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.templates/templatefixedposition/rectangle) | Gets the rectangular area that contains the template field. |



### Example 


This is simplest way to define the field position.
It requires to set a rectangular area on the page that bounds the field value.
All the text that is contained (even partially) into the rectangular area will be extracted as a value:

### See Also
* module [`groupdocs.parser.templates`](..)
* class [`TemplateFixedPosition`](/parser/python-net/groupdocs.parser.templates/templatefixedposition)
* class [`TemplatePosition`](/parser/python-net/groupdocs.parser.templates/templateposition)
