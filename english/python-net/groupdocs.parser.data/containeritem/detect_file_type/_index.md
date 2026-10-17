---
title: detect_file_type method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Detects the file type of the container item."
type: docs
url: /python-net/groupdocs.parser.data/containeritem/detect_file_type/
is_root: false
weight: 1010
---


## detect_file_type {#detection_mode}

Detects the file type of the container item.

```python
def detect_file_type(self, detection_mode):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| detection_mode | `FileTypeDetectionMode` | Defines a mode of the file type detection. |

**Returns:** An instance of `FileType`; `FileType.unknown` if a file type isn't detected.

The `detection_mode` parameter provides the ability to control file type detection:
- **Default** – The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
- **Extension** – The file type is detected only by the file extension.
- **Content** – The file type is detected only by the file content.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import FileTypeDetectionMode

def detect_items(file_path):
    with Parser(file_path) as parser:
        attachments = parser.get_container()
        if not attachments:
            print("Container extraction isn't supported")
            return
        for item in attachments:
            file_type = item.detect_file_type(FileTypeDetectionMode.DEFAULT)
            print(f"{item.name}: {file_type}")
```

### See Also
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem/)
