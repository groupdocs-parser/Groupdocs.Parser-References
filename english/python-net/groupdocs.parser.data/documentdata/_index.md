---
title: DocumentData class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/documentdata/
is_root: false
weight: 20
---

## DocumentData class

Represents data of the document. It consists of [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) objects
which contain field data from document.



The DocumentData type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.data/documentdata/__init__/#list) | Constructs a new instance of DocumentData |
| [__init__](/parser/python-net/groupdocs.parser.data/documentdata/__init__/#groupdocs.parser.templates.Template-list) | Constructs a new instance of DocumentData |


### Properties
| Property | Description |
| :- | :- |
| [count](/parser/python-net/groupdocs.parser.data/documentdata/count) | Gets the total number of the fields data. |
| [template](/parser/python-net/groupdocs.parser.data/documentdata/template) | Gets the template. |



Gets the field data by an index.
### Indexer
| Name | Description |
| :- | :- |
| [index] | The zero-based index of the field. |


### Methods
| Method | Description |
| :- | :- |
| [get_fields_by_name](/parser/python-net/groupdocs.parser.data/documentdata/get_fields_by_name/#System.String) | Returns the collection of field data where the name is equal to `field_name`. |



### Remarks 


An instance of [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata) class is used as return value
of [`Parser.parse_by_template`](/parser/python-net/groupdocs.parser/parser/parse_by_template) and [`Parser.parse_form`](/parser/python-net/groupdocs.parser/parser/parse_form) methods.
See the usage examples there.

### See Also
* module [`groupdocs.parser.data`](..)
* class [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata)
* class [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata)
