---
title: get_container method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts a container object from the document to work with formats that contain attachments, ZIP archives, etc."
type: docs
url: /python-net/groupdocs.parser/parser/get_container/
is_root: false
weight: 1120
---


## get_container

Extracts a container object from the document to work with formats that contain attachments, ZIP archives, etc.

To check if the format supports extracting attachments, see the Supported Document Formats page (Extract Containers and Attachments column): https://docs.groupdocs.com/parser/net/supported-document-formats/

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives
- https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items
- https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios
- https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails
- https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage
- https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files

```python
def get_container(self):
    ...
```

**Returns:** Iterable[ContainerItem] or None: A collection of container items; None if container extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.exceptions import UnsupportedDocumentFormatException

def print_text(item_path, parser):
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(f"{item_path}: {text if text else '[no text]'}")

with Parser("portfolio.pdf") as parser:
    container = parser.get_container()
    if container is None:
        print("Container extraction isn't supported for this format.")
    else:
        for item in container:
            try:
                with item.open_parser() as inner_parser:
                    print_text(item.file_path, inner_parser)
            except UnsupportedDocumentFormatException:
                print(f"{item.file_path}: format is not supported.")
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
