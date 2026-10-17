---
title: parse_form method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Parses the document form."
type: docs
url: /python-net/groupdocs.parser/parser/parse_form/
is_root: false
weight: 1510
---


## parse_form

Parses the document form.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms
- https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template
- https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents

```python
def parse_form(self):
    ...
```

**Returns:** An instance of `DocumentData` containing the extracted data; `None` if parsing by template isn't supported.

### Example

```python
from groupdocs.parser import Parser

file_path = "sample.pdf"
with Parser(file_path) as parser:
    data = parser.parse_form()
    for i in range(data.count):
        field = data[i]
        print(f"{field.name}: ", end="")
        area = field.page_area
        print(area.text if area else "Not a template field")
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
