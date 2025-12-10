---
title: get_fields_by_name method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/documentpagedata/get_fields_by_name/
is_root: false
weight: 20
---

## get_fields_by_name {#System.String}

Returns the collection of field data where the name is equal to `field_name`.


### Returns 


A collection of [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) objects; empty collection if no field data is found.


```python
def get_fields_by_name(self, field_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_name | System.String | The name of the field. |

### Example 


Find fields by a field name:


[`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) class represents field data. Depending on the field [`FieldData.page_area`](/parser/python-net/groupdocs.parser.data/fielddata#page_area) property
can contain any of the inheritors of [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea) class. For example, [`Parser.parse_form`](/parser/python-net/groupdocs.parser/parser/parse_form) method
extracts only text fields.



### See Also
* module [`groupdocs.parser.data`](../../)
* class [`DocumentPageData`](/parser/python-net/groupdocs.parser.data/documentpagedata)
* class [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata)
* class [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea)
