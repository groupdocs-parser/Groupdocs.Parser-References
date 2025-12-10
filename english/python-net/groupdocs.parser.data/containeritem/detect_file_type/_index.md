---
title: detect_file_type method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/containeritem/detect_file_type/
is_root: false
weight: 20
---

## detect_file_type {#groupdocs.parser.options.FileTypeDetectionMode}

Detects a file type of the container item.


### Returns 


An instance of [`FileType`](/parser/python-net/groupdocs.parser.options/filetype) class; [`FileType.Unknown`](/parser/python-net/groupdocs.parser.options/filetype) if a file type isn't detected.


```python
def detect_file_type(self, detection_mode):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| detection_mode | groupdocs.parser.options.FileTypeDetectionMode | Defines a mode of the file type detection. |

### Example 


The following example shows how to detect file type of container item:



### See Also
* module [`groupdocs.parser.data`](../../)
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem)
* class [`FileType`](/parser/python-net/groupdocs.parser.options/filetype)
