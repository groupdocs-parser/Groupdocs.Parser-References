---
title: get_fields_by_name method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Returns the collection of field data where the name is equal to field_name."
type: docs
url: /python-net/groupdocs.parser.data/documentdata/get_fields_by_name/
is_root: false
weight: 1030
---


## get_fields_by_name {#field_name}

Returns the collection of field data where the name is equal to `field_name`.

```python
def get_fields_by_name(self, field_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| field_name | `str` | The name of the field. |

**Returns:** list[FieldData]: A collection of FieldData objects; empty collection if no field data is found.

### Example

```python
# Find fields by a field name
fields = data.get_fields_by_name("InvoiceNumber")
if fields:
    print(f"Found {len(fields)} field(s) named 'InvoiceNumber'")
    for field in fields:
        print(field.text)
else:
    print("InvoiceNumber not found")
```

### See Also
* class [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata/)
