---
title: get_structure method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts a structured text from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_structure/
is_root: false
weight: 1330
---


## get_structure

Extracts a structured text from the document.

Learn more:

- Extract text structure (https://docs.groupdocs.com/display/parsernet/Extract+text+structure)

```python
def get_structure(self):
    ...
```

**Returns:** An instance of `System.Xml.XmlReader` with XML text structure, or `None` if text structure extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.docx") as parser:
    xml_reader = parser.get_structure()
    if xml_reader is None:
        print("Text structure extraction isn't supported")
    else:
        xml_reader.move_to_content()
        xml_content = xml_reader.read_outer_xml()
        # Process xml_content as needed
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
