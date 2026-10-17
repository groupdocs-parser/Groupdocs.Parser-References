---
title: get_metadata_value method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Gets the metadata value."
type: docs
url: /python-net/groupdocs.parser.data/containeritem/get_metadata_value/
is_root: false
weight: 1030
---


## get_metadata_value {#name}

Gets the metadata value.

```python
def get_metadata_value(self, name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| name | `str` | The name of the metadata. |

**Returns:** str or None: The value of the metadata item, or None if the metadata with this name isn't found.

### Example

```python
    from groupdocs.parser import Parser

    with Parser("archive.zip") as parser:
        for item in parser.get_container() or []:
            print(item.name, item.get_metadata_value("author"))
    ```

### See Also
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem/)
