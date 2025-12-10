---
title: from_extension method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/filetype/from_extension/
is_root: false
weight: 30
---

## from_extension {#System.String}

Maps file extension to file type.


### Returns 


When file type is supported returns it, otherwise returns default [`FileType.Unknown`](/parser/python-net/groupdocs.parser.options/filetype) file type.


```python
def from_extension(self, extension):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| extension | System.String | File extension (including the period "."). |
### Exceptions
| Exception | Description |
| :- | :- |
| ArgumentException | Thrown when `extension` is null or empty string. |





### See Also
* module [`groupdocs.parser.options`](../../)
* class [`FileType`](/parser/python-net/groupdocs.parser.options/filetype)
