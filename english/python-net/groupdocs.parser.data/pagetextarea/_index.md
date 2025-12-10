---
title: PageTextArea class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/pagetextarea/
is_root: false
weight: 150
---

## PageTextArea class

Represents a page text area which is used to represent a text value in the parsing by template or parsing form functionality.



**Inheritance:** [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) → 
[`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea)



The PageTextArea type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/pagetextarea/__init__/#System.String-groupdocs.parser.data.Page-groupdocs.parser.data.Rectangle) | Initializes a new instance of the [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) class. |
| [__init__](/parser/python-net/groupdocs.parser.data/pagetextarea/__init__/#System.String-System.Nullable`1[[System.Double]]-groupdocs.parser.data.TextStyle-groupdocs.parser.data.Page-groupdocs.parser.data.Rectangle) | Constructs a new instance of PageTextArea |
| [__init__](/parser/python-net/groupdocs.parser.data/pagetextarea/__init__/#list-groupdocs.parser.data.Page) | Constructs a new instance of PageTextArea |


### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.data/pagetextarea/rectangle) | Gets the rectangular area. |
| [page](/parser/python-net/groupdocs.parser.data/pagetextarea/page) | Gets the document page information such as page index and page size. |
| [text](/parser/python-net/groupdocs.parser.data/pagetextarea/text) | Gets the text. |
| [base_line](/parser/python-net/groupdocs.parser.data/pagetextarea/base_line) | Gets the base line. |
| [text_style](/parser/python-net/groupdocs.parser.data/pagetextarea/text_style) | Gets the text style such as font size, font name an so on. |
| [areas](/parser/python-net/groupdocs.parser.data/pagetextarea/areas) | Gets the collection of child text page areas. |



### Remarks 


An instance of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) class is used as return value
of the following methods:

|
|
 |
 |
 |
 |



Also an instance of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) class is used as value
of [`FieldData.page_area`](/parser/python-net/groupdocs.parser.data/fielddata#page_area) property.



See the usage examples there.



The text area can be single or composite. 
In the first case it contains a text which is bounded by a rectangular area. 
In the second case it contains other text areas; text and table properties are calculated by child text areas.

### See Also
* module [`groupdocs.parser.data`](..)
* class [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea)
* class [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea)
