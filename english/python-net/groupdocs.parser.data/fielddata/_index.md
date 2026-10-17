---
title: FieldData class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents field data such as a name, a page index, a field value, and possibly other types like text, image, or table."
type: docs
url: /python-net/groupdocs.parser.data/fielddata/
is_root: false
weight: 50
---


## FieldData class

Represents field data such as a name, a page index, a field value, and possibly other types like text, image, or table.

The instances of [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata/) class are used in [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata/) collection.

The FieldData type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/fielddata/__init__/#name-page_area-linked_data_field) | Initializes a new instance of the [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata/) class with UPPER CASE name. |
| [__init__](/parser/python-net/groupdocs.parser.data/fielddata/__init__/#name-page_area-linked_data_field-use_upper_case_name) | Initializes a new FieldData instance. |
| [__init__](/parser/python-net/groupdocs.parser.data/fielddata/__init__/#name-page_area) | Initializes a new instance of the [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata/) class with UPPER CASE name. |
| [__init__](/parser/python-net/groupdocs.parser.data/fielddata/__init__/#name-page_area-use_upper_case_name) | Initializes a new instance of the [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata/) class. |

### Properties
| Property | Description |
| :- | :- |
| [linked_field](/parser/python-net/groupdocs.parser.data/fielddata/linked_field/) | The linked field. |
| [name](/parser/python-net/groupdocs.parser.data/fielddata/name/) | The field name. An uppercase string value that represents the name of the field. |
| [page_area](/parser/python-net/groupdocs.parser.data/fielddata/page_area/) | The page area of the field. |
| [page_index](/parser/python-net/groupdocs.parser.data/fielddata/page_index/) | The zero-based index of the page that contains the field. |
| [text](/parser/python-net/groupdocs.parser.data/fielddata/text/) | The text of the field as a str; None if [`FieldData.page_area`](/parser/python-net/groupdocs.parser.data/fielddata/page_area/) property isn't a [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea/). |
| [use_upper_case_name](/parser/python-net/groupdocs.parser.data/fielddata/use_upper_case_name/) | The boolean value indicates whether a `Name` was converted to UPPER CASE. |

### See Also
* module [`groupdocs.parser.data`](/parser/python-net/groupdocs.parser.data/)
