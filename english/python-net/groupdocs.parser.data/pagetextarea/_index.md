---
title: PageTextArea class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents a page text area which is used to represent a text value in the parsing by template or parsing form functionality."
type: docs
url: /python-net/groupdocs.parser.data/pagetextarea/
is_root: false
weight: 160
---


## PageTextArea class

Represents a page text area which is used to represent a text value in the parsing by template or parsing form functionality.

An instance of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea/) class is used as return value of the following methods:

- [`Parser.get_text_areas`](/parser/python-net/groupdocs.parser/parser/get_text_areas/)
- `Parser.get_text_areas(PageTextAreaOptions)`
- `Parser.get_text_areas(int)`
- `Parser.get_text_areas(int, PageTextAreaOptions)`

Also an instance of [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea/) class is used as value of [`FieldData.page_area`](/parser/python-net/groupdocs.parser.data/fielddata/page_area/) property.

See the usage examples there.

The text area can be single or composite. In the first case it contains a text which is bounded by a rectangular area. In the second case it contains other text areas; text and table properties are calculated by child text areas.

The PageTextArea type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/pagetextarea/__init__/#text-page-rectangle) | Initializes a new PageTextArea instance. |
| [__init__](/parser/python-net/groupdocs.parser.data/pagetextarea/__init__/#text-base_line-text_style-page-rectangle) | Initializes a new PageTextArea. |
| [__init__](/parser/python-net/groupdocs.parser.data/pagetextarea/__init__/#areas-page) | Initializes a new PageTextArea instance. |

### Methods
| Method | Description |
| :- | :- |
| [to_string](/parser/python-net/groupdocs.parser.data/pagetextarea/to_string/) | Converts the value of this instance to a string. |

### Properties
| Property | Description |
| :- | :- |
| [areas](/parser/python-net/groupdocs.parser.data/pagetextarea/areas/) | The collection of child text page areas. |
| [base_line](/parser/python-net/groupdocs.parser.data/pagetextarea/base_line/) | The base line of the page text area. |
| [text](/parser/python-net/groupdocs.parser.data/pagetextarea/text/) | The text of the page area as a string. |
| [text_style](/parser/python-net/groupdocs.parser.data/pagetextarea/text_style/) | The text style of the page area, such as font size, font name, and so on. |
| [page](/parser/python-net/groupdocs.parser.data/pagearea/page/) | The document page information such as page index and page size. (inherited from [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea/)) |
| [rectangle](/parser/python-net/groupdocs.parser.data/pagearea/rectangle/) | The rectangular area of the page as a [`Rectangle`](/parser/python-net/groupdocs.parser.data/rectangle/). (inherited from [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea/)) |

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)
