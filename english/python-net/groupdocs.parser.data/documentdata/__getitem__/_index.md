---
title: DocumentData indexer
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/documentdata/__getitem__/
is_root: false
weight: 30
---

## DocumentData indexer


Gets the field data by an index.
### Indexer
| Name | Description |
| :- | :- |
| index | The zero-based index of the field. |



### Returns 


An instance of [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) class.

### Example 


Iteration via all the fields:


[`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) class represents field data. Depending on the field [`FieldData.page_area`](/parser/python-net/groupdocs.parser.data/fielddata#page_area) property
can contain any of the inheritors of [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea) class. For example, [`Parser.parse_form`](/parser/python-net/groupdocs.parser/parser/parse_form) method
extracts only text fields:

### See Also
* module [`groupdocs.parser.data`](../../)
* class [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata)
* class [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata)
* class [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea)
