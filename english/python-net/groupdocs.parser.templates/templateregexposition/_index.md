---
title: TemplateRegexPosition class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templateregexposition/
is_root: false
weight: 110
---

## TemplateRegexPosition class

Provides a template field position which uses the regular expression.



**Inheritance:** [`TemplateRegexPosition`](/parser/python-net/groupdocs.parser.templates/templateregexposition) → 
[`TemplatePosition`](/parser/python-net/groupdocs.parser.templates/templateposition)



The TemplateRegexPosition type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.templates/templateregexposition/__init__/#System.String) | Initializes a new instance of the [`TemplateRegexPosition`](/parser/python-net/groupdocs.parser.templates/templateregexposition) class. |
| [__init__](/parser/python-net/groupdocs.parser.templates/templateregexposition/__init__/#System.String-bool) | Initializes a new instance of the [`TemplateRegexPosition`](/parser/python-net/groupdocs.parser.templates/templateregexposition) class. |


### Properties
| Property | Description |
| :- | :- |
| [expression](/parser/python-net/groupdocs.parser.templates/templateregexposition/expression) | Gets the regular expression. |
| [match_case](/parser/python-net/groupdocs.parser.templates/templateregexposition/match_case) | Gets the value that indicates whether a text case isn't ignored. |



### Example 


The following example shows the situation
if the document contains "Invoice Number INV-12345" then template field can be defined in the following way:




In this case as a value the entire string is extracted.
To extract only a part of the string the regular expression group "value" is used:



In this case as a value "INV-3337" string is extracted.

### See Also
* module [`groupdocs.parser.templates`](..)
* class [`TemplatePosition`](/parser/python-net/groupdocs.parser.templates/templateposition)
* class [`TemplateRegexPosition`](/parser/python-net/groupdocs.parser.templates/templateregexposition)
