---
title: TemplateField class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the template text field."
type: docs
url: /python-net/groupdocs.parser.templates/templatefield/
is_root: false
weight: 40
---


## TemplateField class

Provides the template text field.

Text fields are defined by its position on the page. There are three ways to define a text field:

- [`TemplateFixedPosition`](/parser/python-net/groupdocs.parser.templates/templatefixedposition/) Using the rectangular area
- [`TemplateRegexPosition`](/parser/python-net/groupdocs.parser.templates/templateregexposition/) Using the regular expression
- [`TemplateLinkedPosition`](/parser/python-net/groupdocs.parser.templates/templatelinkedposition/) Using the linked field

The TemplateField type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatefield/__init__/#position-name) | Initializes a new TemplateField instance. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatefield/__init__/#position-name-page_width) | Initializes a new TemplateField. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templatefield/__init__/#position-name-page_width-use_upper_case_name) | Initializes a new TemplateField. |

### Methods
| Method | Description |
| :- | :- |
| [scale](/parser/python-net/groupdocs.parser.templates/templatefield/scale/#factor) | Scales the template item by a given factor. |
| [scale_double](/parser/python-net/groupdocs.parser.templates/templatefield/scale_double/) |  |

### Properties
| Property | Description |
| :- | :- |
| [is_hidden](/parser/python-net/groupdocs.parser.templates/templatefield/is_hidden/) | The hidden template field flag. |
| [position](/parser/python-net/groupdocs.parser.templates/templatefield/position/) | The position describes how to find the template field on the document page. |
| [value](/parser/python-net/groupdocs.parser.templates/templatefield/value/) | The value of the template field. |
| [name](/parser/python-net/groupdocs.parser.templates/templateitem/name/) | The name of the template item. Uppercase string value representing the template item's name. (inherited from [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/)) |
| [page_width](/parser/python-net/groupdocs.parser.templates/templateitem/page_width/) | The width of the page in pixels; None if the page width is unknown. (inherited from [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/)) |
| [use_upper_case_name](/parser/python-net/groupdocs.parser.templates/templateitem/use_upper_case_name/) | The property returns a boolean value that indicates whether a Name was converted to UPPER CASE. (inherited from [`TemplateItem`](/parser/python-net/groupdocs.parser.templates/templateitem/)) |

### See Also
* module [`groupdocs.parser.templates`](/parser/python-net/groupdocs.parser.templates/)
